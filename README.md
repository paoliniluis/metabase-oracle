Contents of this docker-compose
===============================


This is the old school Metabase + postgreSQL as the Application database with an Oracle DB.

- Metabase is exposed through port 8443
- PosgreSQL is exposed through port 5432

both containers are in the same metanet1 network and you can wipe postgreSQL database by doing sudo `rm -rf /postgres_origin` on this folder (/environments/postgres)

NOTES:
- a drivers folder is there so you can leave the ojdbcxx.jar driver in case you need to replace the Oracle driver


To run this lab
- do "docker compose up --build" on the root folder