#EC OracleDB Node Installation Process for a dummy App

##Installation
1. Go to http://www.oracle.com/technetwork/topics/linuxx86-64soft-092277.html, download these two files (instantclient-basic-linux.x64-12.1.0.2.0.zip, instantclient-sdk-linux.x64-12.1.0.2.0.zip) - your Oracle versions might vary - exmplaes are for this is for 12c
  * Instant Client Package - Basic: All files required to run OCI, OCCI, and JDBC-OCI applications 
  * Instant Client Package - SDK: Additional header files and an example makefile for developing Oracle applications with Instant Client
2. Unzip these files above locally, it will generate a folder 'instantclient_x_x', rename the folder to 'instantclient'.
3. Copy 'Instantclient' directory to the application root directory
4. Make the appropriate changes to manifest.yml and if required, to the shell script as well.
5. After a 'cf login', do 'cf push'.

##Usage
* modify the server-dummy.js for your implementation (see the instruction "app begins here")

##Reference
* https://github.com/oracle/node-oracledb
