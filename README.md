
WELCOME
=======
The goal of this module to enable the request of a resource at any point in a flow. This resource can be a file, a message (from VM, JMS, AMQP, etc.), an e-mail, etc. It's intended for resources than originally can only requested by message sources.

Some of its common use cases are:

- Load a file in the middle of a flow for processing.
- Consume messages (one, N, all) from a queue in the middle of a flow.
- Pull messages from a mail server on demand, to use its data in an enricher for example.

Usage
-----
```xml
<mulerequester:request config-ref="" resource="" timeout="" returnClass="" throwExceptionOnTimeout="" />
```

Request a resource from an address or endpoint. 
To make the request using the address, use the format "protocol://address". E.g.: "file://path/to/file". 
Otherwise, you can use a global endpoint name. E.g.: "fileEndpoint". 
{@sample.xml ../../../doc/MuleRequester-connector.xml.sample mulerequester:request}

Parameters:
resource The address of the resource or the global endpoint name
timeout The timeout to wait for when requesting the resource (optional - default 1000 ms)
returnClass The return class to which this processor will transform the payload from the requested resource (optional)
throwExceptionOnTimeout Whether to throw an exception or not if no message is received in the configured timeout (optional - default false)
Returns:
the payload from the requested resource


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
