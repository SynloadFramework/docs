Databases Included With Synload Framework
=========================================

MySQL
-----
Included with SF by default is a mysql jdbc connector. Can be enabled in the configuration file. ::

	/projectRoot/config.ini
	
The settings :: 

	dbenabled=false
	jdbc=jdbc\:mysql\://127.0.0.1\:3306/%dbname?useUnicode\=true&characterEncoding\=UTF-8&autoReconnect\=true
	dbuser=%username
	dbpass=%password
	
SQL Manager
+++++++++++
If you have a module that requires the automatic installation of tables into the database, then you will need to enable this option.

dbenabled
+++++++++
This setting will enable and disable the mysql connector, it will attempt to connect to the mysql server on server start.

Change this to ``true`` if you want to use mysql

dbuser
++++++
This variable defines the user that will be used to connect to the database instance. ::

	Replace %username with the connection username.
	
dbpass
++++++
This variable defines the password used in combination with the user name above. ::

	Replace %password with the connection password.

jdbc
++++
`Information on JDBC connection strings <https://en.wikipedia.org/wiki/Java_Database_Connectivity>`_ ::

	Replace %dbname with the name of the database on the server

Neo4J
-----

Included with SF. Can be enabled within the config file in the root project directory. ::

	/projectRoot/config.ini
	
This file