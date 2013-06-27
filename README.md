ZooServer
=========

ECF Discovery Server based on Zookeeper


Building
========

git clone https://github.com/ECF/ZooServer.git
cd ZooServer/org.eclipse.ecf.zooserver.parent
mvn clean install

Starting
========

cd ..
cd org.eclipse.ecf.zooserver.parent/target/products

This directory contains various zips for various platforms. Unzip the server
for your platform. Enter the directory and run the zooserver executable.

The server is now ready to receive OSGi remote service publications and publish these to
attached clients.
