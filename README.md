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

