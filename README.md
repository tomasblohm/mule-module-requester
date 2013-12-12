
WELCOME
=======
Congratulations you have just created a new Mule Module!

This wizard created a number of new classes and resources useful for Mule
modules.  Each of the created files contains documentation and TODO
items where necessary.  Here is an overview of what was created.

./pom.xml:
A maven project descriptor that describes how to build this module.

./LICENSE.md:
The open source license text for this project.

TESTING
=======

This  project also contains test classes that can be run as part of a test
suite.

ADDITIONAL RESOURCES
====================
Everything you need to know about getting started with Mule can be found here:
http://www.mulesoft.org/documentation/display/MULE3INTRO/Home

There further useful information about extending Mule here:
http://www.mulesoft.org/documentation/display/DEVKIT/Home

Remember if you get stuck you can try getting help on the Mule user list:
http://www.mulesoft.org/email-lists

Also, MuleSoft, the company behind Mule, offers 24x7 support options:
http://www.mulesoft.com/enterprise-subscriptions-and-support

INSTALLATION
============
For MuleStudio
--------------
1. Download the update site zip file from the following location, replacing {version} with the desired one:
https://repository-master.mulesoft.org/nexus/content/repositories/releases/org/mule/modules/mule-module-requester/{version}/mule-module-requester-{version}-studio-plugin.zip
2. Install it in MuleStudio as a regular update site from a file. The module will appear under the Components tab.

For Maven
---------
```xml
<dependency>
    <groupId>org.mule.modules</groupId>
    <artifactId>mule-requester</artifactId>
    <version>{version}</version>        
</dependency>
```  

Enjoy your Mule ride!

The Mule Team
