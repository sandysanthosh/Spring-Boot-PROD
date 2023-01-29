#### There are several ways to check production logging in a Spring Boot application, some of which include:

* Using a logging framework such as Logback or Log4j: These frameworks can be configured to write log statements to a file or send them to a remote logging service such as Loggly or Elasticsearch.

*  Using Spring Boot Actuator: Spring Boot Actuator provides a set of endpoints that can be used to monitor and manage a Spring Boot application. One of these endpoints, /actuator/logfile, can be used to view the contents of the application's log file.

*  Using a log management tool: Tools such as the Elastic Stack, Logstash, and Fluentd can be used to collect, process, and analyze log data from a Spring Boot application.

*  You can also set up the logging level to ERROR,WARN,INFO,DEBUG,TRACE to check the logging in production.

*  You may also want to look into using the Spring Cloud Sleuth for distributed tracing, which allows you to trace the flow of a request through a system of microservices.

# LOG4J-java

      -logging API for java.

Advantage:

      Quick Debugging
      Problem Diagnosis ->  production 
      Easy Maintenance
      Cost and Time Savings


#### log level:

      import org.apache.log4j.*;  

      private static org.apache.log4j.Logger log = Logger.getLogger(LogClass.class);  

      ALL < TRACE < DEBUG < INFO < WARN < ERROR < FATAL < OFF  

      fatal
      error
      warn
      info
      debug

search for error-> direction->up`

#### LOG4J:

    logger.info
    logger.fatal
    logger.debug
    logger.notify
    logger.notifyall
    logger.error
    logger.equals
    logger.tostring

#### POM.xml:

        <dependency>
            <groupId>org.apache.logging.log4j</groupId>
            <artifactId>log4j-core</artifactId>
            <version>2.12.1</version>
        </dependency>

