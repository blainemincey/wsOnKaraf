wsOnKaraf: Demonstrates a SOAP Web service with CXF
======================================================
SOAP Web Service on Karaf

Steps to deploy/run

1.  git clone https://github.com/blainemincey/wsOnKaraf.git

2.  cd wsOnKaraf

3.  mvn install

4.  Start Fuse --> <fuseHomeDirectory>/bin/fuse

5.  In Fuse Terminal, JBossFuse:admin@root> install -s mvn:com.jboss/wsOnKaraf/0.0.1-SNAPSHOT

6.  Should receive output similar to --> Bundle ID:  279

7.  To verify that it deployed, do a JBossFuse:admin@root> list

8.  Last entry should be similar to this --> [ 279] [Active     ] [Created     ] [   80] JBoss Fuse Quickstart: soap (0.0.1.SNAPSHOT)

9.  To test, go back to project directory.  Do a mvn -Ptest.  Should receive a Hello Blaine Mincey response.

10. To test with something like SOAP-UI, use this WSDL http://localhost:8181/cxf/HelloWorld?wsdl .

