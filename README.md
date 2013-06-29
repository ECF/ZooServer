ZooServer
=========

ECF Discovery Server based on Zookeeper

Binaries
========

Prebuild binaries can be picked up from [zoobin].

[zoobin]: http://download.ecf-project.org/repo/C-HEAD-discovery.zooserver/builds/lastSuccessfulBuild/archive/org.eclipse.ecf.zooserver.product/target/products/ "zooserver build"

Building
========

git clone https://github.com/ECF/ZooServer.git

cd ZooServer/org.eclipse.ecf.zooserver.parent

mvn clean install

Starting
========

cd ../org.eclipse.ecf.zooserver.parent/target/products

This directory contains various zips for various platforms. Unzip the server for your platform. Enter the directory and run the zooserver executable.

The server is now ready to receive OSGi remote service publications and publish these to attached clients.

Logging
=======

If you get log4j errors then you are probably not running from the root of the server. Please update the zooserver.ini file to point the log4j.properties file to a absolute location.

e.g: 

-Dlog4j.configuration=file:/c:/my/folder/log4j.properties
