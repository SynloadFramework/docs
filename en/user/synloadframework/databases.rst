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
	
dbenabled
+++++++++
This setting will enable and disable the mysql connector, it will attempt to connect to the mysql server on server start.

Change this to *true* if you want to use mysql

Neo4J
-----

Included with SF. Can be enabled within the config file in the root project directory. ::

	/projectRoot/config.ini
	
This file