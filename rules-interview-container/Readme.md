Introduction
============
This quickstart demonstrates the usage of a rules service which performs an age check.  
The drl resource is specified using annotations within the InterviewRules interface.       
The name of the service in the drl is specified using a Mapping annotation containing an MVEL expression.

This quickstart also demonstrates how a domain property can be made available as a global variable inside your DRL.
See references to ${user.name} (system property) mapping to userName (domain property) mapping to userName (global variable) inside switchyard.xml.
Then look at Interview.drl and how the userName global variable is used in the DRL.

This rules-interview-container quickstart differs from the rules-interview quickstart.
A /META-INF/kmodule.xml is used, which is referenced by both the <container> element in switchyard.xml, and the KIE/Drools container.
The rules-interview quickstart, on the other hand, manually lists the required resource.

![Rules Interview Container Quickstart](https://github.com/jboss-switchyard/quickstarts/raw/master/rules-interview-container/rules-interview-container.jpg)


Preqrequisites 
==============
Maven

Running the quickstart
======================

JBoss AS 7
----------
1. Build the quickstart:

        mvn clean install

2. Run the test:

        mvn -Dtest=RulesInterviewTest test

Expected Output:
================
(userName is a placeholder in this Readme.)
```
Running org.switchyard.quickstarts.rules.interview.RulesInterviewTest  
********** Twenty is a valid applicant, userName. **********  
Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 3.131 sec`  
```

## Further Reading

1. [Configuration Documentation](https://docs.jboss.org/author/display/SWITCHYARD/Configuration)
2. [Rules Service Documentation](https://docs.jboss.org/author/display/SWITCHYARD/Rules)
