FROM metabase/metabase-enterprise:v1.47.3

ADD groupSetup.sh .
RUN sh groupSetup.sh

ADD https://download.oracle.com/otn-pub/otn_software/jdbc/217/ojdbc8.jar /plugins/oracle.metabase-driver.jar

RUN chown metabase:metabase /plugins/oracle.metabase-driver.jar