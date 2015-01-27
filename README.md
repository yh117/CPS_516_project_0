# CPS_516_project_0


####  1  Azure SQL Cloud Platform        

##### pros:
 1.  Offers one-month free trial and $200 credit on Azure services during the trial. [1]   
 2.  Supports hybrid storage: solutions to integrate your own datacenters with Azure cloud to leverage on-premises performance and lower the cost in the cloud. [2]   
 3.  Scalable, performance predictable, self-managed for near-zero maintenance. [3]   

####  2  Oracle        

##### pros:
 1.  Supports HA clustering, load balancing and scalability for Oracle RAC. [4]   
 2.  Provides one of the best database cloning and one of the best DR solutions (Oracle's Data Guard, RMAN). [4]   
 3.  Reader and writer don't block each other. [4]   
 4.  Supports extended stored procedures. Supports Java to write stored procedures. [4]   
 5.  Features can be customized to fit specific application. [14]    

##### cons:
 1.  Need to buy licenses for each computer that you want to use Oracle database on. [14]    
 2.  Learning curve is steep. [14]    

####  3  MS SQL Server       

##### pros:
 1.  MS SQL Server Cluster provides HA failover. [4]   
 2.  Uses row versioning to achieve snapshot isolation, reader and writer don't block each other. [4]   
 3.  Supports extended stored procedures. [4]   

##### cons:
 1.  No load balance for MS SQL Server Cluster. [4]   
 2.  No scalability at the instance level. [4]   
 3.  Only runs on Windows      

####  4  SAP Sybase ASE        

##### pros:
 1.  Suports HA clustering, load balancing and scalability. [4]   
 2.  Provides best replication solution. Replication can be done at different levels (database level, transaction level, table level, stored procedure level, function string level). Supports both heterogeneous and homogeneous replication. [4]   
 3.  Supports stored procedures, and supports Java to write stored procedures. [4]   

##### cons:
 1.  Reader and writer block each other. [4]   

####  5  SAP Sybase IQ       

##### pros:
 1.  SAP Sybase IQ is a column-based (very fast query speed, index for all columns, data compression), petabyte scale, relational database. [4]   
 2.  Supports snapshot versioning, reader and writer don't block each other. [4]   
 3.  Achieved world’s Largest Data Warehouse Guinness World Record 12.1 PB. [15]    

##### cons:
 1.  Needs a reasonable size of data to benefit from Sybase IQ (> 200GB). [22]    
 2.  Inefficient to do row insertion. [22]    

####  6  TeraData        

##### pros:
 1.  Provides text analytics functionality to track unstructured data. [5]   
 2.  TeraData is a networked/distributed DB platform. [4]   

####  7  MySQL Cluster       

##### pros:
 1.  Claimed higher TPC-C performance benchmarks than Oracle RAC, uses an in-memory storage engine (by choose memory option). [4]   
 2.  Applications communicate with MySQL servers which do not store any data, and MySQL servers communicate with data nodes. This architecture makes scalability easy. [24]    
 3.  Features shared-nothing clustering, auto sharding, synchronous replication (also supports asynchronous replication functionality between different data centers). Provides SQL and NoSQL APIs (provide direct access to data without a SQL layer). [23]    

##### cons:
 1.  Some operations may be slow due to distributed nature. [24]    

####  8  MySQL       

##### pros:
 1.  MySQL is Written in C and C++ and is the second most popular open source database, one component of LAMP. Supports stored procedures, triggers, cursors. [26]    
 2.  Development process is more organized by Oracle and new features are added. [25]    

##### cons:
 1.  MySQL is not as mature as other RDBMS (not feature-rich enough), and may be close source in the future. MySQL is not community driven but owned by Oracle and some modules are no longer open source. The community driven fork of MySQL is called MariaDB. [25]    

####  9  IBM DB2       

##### pros:
 1.  DB2 is a family of database server product. Some products support object-relational and non-relational structures. [27]    
 2.  DB2 works very well with IBM’s pSeries/Power server and Veritas VCS/Sun Cluster. [4]   
 3.  Supports object tables, before triggers, Java method, multiple user-defined functions and arrays. BD2 provides Self-Tuning Memory Management feature which optimizes performance based on workload. [28]    

####  10   Redis       

##### pros:
 1.  Redis is an open-source, In-memory, K/V store with optional persistence (syncs data to disk in every 2 seconds by default). Replication is built on a master-slave architecture. Data in server can replicate to slave(s). [6], [20] 
 2.  Besides string, Redis also supports lists, sets, sorted set, hashes. Supports high level atomic operations on these data structures. If master wipes out, one slave will be promoted to become the master. [20]    

##### cons:
 1.  Compared to Memcached, Redis is hard to configure. [21]    
 2.  The failover strategy needs a SENTINEL, and if the SENTINEL and master both fail, the whole system fails. [21]    

####  11   Riak        

##### pros:
 1.  Riak is a distributed, replicated, Key/Vvalue databse that offers extremely high availability, fault tolerance, operational simplicity and scalability. Riak is written in Erlang. [6], [29] 
 2.  Riak provides a RESTful API and other features including secondary indexes, Solr client query APIs and MapReduce (written in JavaScript and submitted by REST API), latency prediction. [29]    

##### cons:
 1.  Since there is no custom front-end, submissions may be lost when connections between client and Riak cluster. [30]    

####  12   Memcached       

##### pros:
 1.  Memcached is a free, open-source, distributed, memory based Key/Value database. [6]   
 2.  Memcached system is based on a client-server architecture. All the servers are in a flat structure, and the clients use a hashtable to determine which server to connect to based on the key of the data. The server will use another hashtable to find the corresponding data. [19]    
 3.  Memcached features low complexity and is simple to confiture, extremely stable. [16]    

##### cons:
 1.  Presistence of data is not guaranteed. When the memory is full, the ordest data will be deleted. [19]    
 2.  Memcached can only store string. [21]    
 3.  Needs a full system restart to solve unbalanced clusters. [21]    

####  13   Cassandra       

##### pros:
 1.  Cassandra is based on BigTable and DynamoDB. [6]   
 2.  Cassandra is open source, hydrid key-value and column based, distributed database. There is no master cluster, every node in the cluster has the same role. Cassandra introduces a new query language CQL (Cassandra Query Language), which is a SQL-like alternative to the traditional RPC interface. [31]    

####  14   HBase       

##### pros:
 1.  Data store for Apache Hadoop based on ideas from BigTable. [6]   
 2.  Some popular usage cases for column based data stores are: keeping unstructured, non volatile information, scaling. [6]   

##### cons:
 1.  HBase is memory-hungry compared with Cassandra and Riak. HBase Requires disabling the table when changing Schema which means maintenance window. [30]    

####  15   Couchbase       

##### pros:
 1.  Couchbase is an open source, distributed (shared nothing architecture, every node has a cluster manager (for operations like replication and rebalancing) and a data manager(for data storing and querying) ), scalable, document based (JSON, schema less) databse optimized for interactive applications. Suport REST API. New data only append to the existing data to ensure data integrity. [6], [101]    

##### cons:
 1.  Couchbase requires a rolling restart of the nodes after schema changed. [6]     

####  16   CouchDB       

##### pros:
 1.  CouchDB stores data in JSON documents, queries the databse in browser through HTTP. [7]   
 2.  CouchDB is a schema-free, distributed, document based database, a CouchDB document is a JSON object that contains various fields. [8]   

####  17   MongoDB       

##### pros:
 1.  MongoDB is a free and open-source document based (JSON style) databse written in C. [10]    
 2.  Features schema free/flexible schema, ease of scale-out, index on any attribute, replication & high availability, auto-sharding, rich queries, fast in-place updates, [9], [12] 

##### cons:
 1.  No joins, more memory needed to store key for each document, reader-writer lock. Transactions bewteen multiple files are not atomic. [11]    

####  18   OrientDB        

##### pros:
 1.  OrientDB is an open source, light, document based (JSON), graph (compliant with TinkerPop Blueprints standard) database management system written in JAVA (and therefore is cross platform). OrientDB is built on a new indexing algorithm called MVRB-Tree which is a combination of red black tree and B+tree. OrientDB Supports schema-less, schema-full and schema-mixed modes. OrientDB also supports ACID transactions, HTTP, RESTful protocol, SQL and its own eSQL. [32]    

##### cons:
 1.  Bulk inserts may cause out-of-memory crash. [35]    

####  19   ArangoDB        

##### pros:
 1.  ArangoDB is an open source, mostly-memory (store data in disk while keep index and data in memory) document based (JSON), graph database written in C++. Supports ACID, multiple database, replication, HTTP REST API, stored procedure functionality (can be written in Javascript and framework is lightweight). Keeps journal files and only append to the end. Since the already written part of the journal files are never modifies, ArangoDB can restore data based on the journal files. ArangoDB saves documents which have the same attributes together (as a collection), and saves their attribute names and types only once (for a collection, this is called shape) to reduce the memory usage. [33]    

####  20   Neo4J       

##### pros:
 1.  Neo4J is an open source, embedded, disk-based, fully transitional, graph database written in JAVA. Neo4J stores data in either and edge, a node or an attribute. The edge and node can have any number of attributes and can be labelled. The labels can be used for searchinig to reduce the search scope. [34]    
 2.  Neo4J is schema-free, graph based data store written in Java. [6]   

##### cons:
 1.  Can not shard Neo4J therefore all database is in the same saver. Neo4J and other graph database is not recommended if foreign key is required. If the original database contains complicated SQL, then migration to graph database is difficult. [36]    

####  21   ElasticSearch       

##### pros:
 1.  ElasticSearch is an open source, distributed (indices are in shards and each shard can have zero or more replicas, auto-rebalancing), document based (JSON), schema-free, full-text search (supports all kinds of documents) server based on Lucene written in Java. Supports HTTP RESTful interface, multienancy (can have multiple indices) and persistent index store (index can be restored after a server crash. This feature is called gateway). [37]    
 2.  ElasticSearch provides real-time search (latency is just milliseconds after adding or updating the document) and can dynamically add or remove nodes. [40]    

##### cons:
 1.  When index is large, index update takes time and may fail. Biiger workload compared to common databse. [40]    

####  22   Accumulo        

##### pros:
 1.  Accumulo is an open source, distributed, key/value database based on BigTable, Hadoop, ZooKeeper and Trift written in Java. Supports server-side programming (implements MapReduce operation to aggregate data), cell-level security (each key/value pair has its security label stored in the column to control the accessibility of data (column visibility can be different in the same table) for different users.). [38], [39] 
 2.  Accumulo doesn't need to specify columns in advance which makes Accumulo database more convenient to add columns. Supports off-heap in-memory map (stores recently written data which makes it less susceptible to Java GC and more efficient on writing data). [41]    

##### cons:
 1.  Accumulo has smaller user group compared to Hbase. [41]    

####  23   Scalaris        

##### pros:
 1.  Scalaris is an open source, scalable, transactional (first NoSQL that supports ACID for multi-key transactions), distributed (can add or remove server on the fly), key/value database written in Erlang. Supports replication and fail-ove, self-management, automatic data partitioning. [42], [43] 

####  24   VoltDB        

##### pros:
 1.  VoltDB is an in-memory, scalable databased. Supports ACID, SQL, Java stored procedure (the minimum transaction), horizontal patitioning in an individual hardware, k-safety (replication), continuous snapshots and command logging (which is used for data restore). Has two versions, e.g. enterprise version and community version. Community version is free software. [44], [45] 

##### cons:
 1.  Although users can change stored procedure on the fly, changing schema or reconfiguring need to shutdown the database. No WAN support (in network partition, VoltDB will be unavailable to make consistency possible). VoltDB is not for OLAP, since OLAP needs locks and affect performance. [46]    

####  25   Aerospike       

##### pros:
 1.  Aerospike is an open source, falsh optimized (index stored in RAM and data stored in large block), in-memory, key/value database written in C. Aerospike is built on 3 layers, e.g. a flash optimized data layer, a self-managed distribution layer (this layer is replicated between different servers to achieve consistency) and a cluster-aware client layer (used for server configuration checking and server communication management). Latency for 99.9% operations are within 5 milliseconds. [47], [48] 

##### cons:
 1.  Aerospike is written in C, so there is no garbage collection which has potential risk of memory leak. [48]    

####  26   Kyoto Tycoon        

##### pros:
 1.  Kyoto Tycoon is a lightweight, multithreaded, high available (hot backup, updata logging), key/value database server written in C++. Kyoto Tycoon is compatible with SQLite. Supports transactional operation (but not fully transactional), auto expiration mechanism (deals with cache data and persistent data management), HTTP REST interface and RPC interface, stored procedure feature (in Lua). [49], [50] 

##### cons:
 1.  Kyoto Tycoon only supports C++, Lua API. [50]    

####  27   PostgreSQL        

##### pros:
 1.  PostgreSQL is a free, open source, object-relational database management system (a child table can inherit characteristics from a parent table). Highly compliant wth SQL:2011 standard. Supports ACID, MVCC (offers a snapshot to each transacion and avoids locking which enable a very good concurrency performance), built-in binary replication (replicates to slaves and supports read operations on slaves), rich data type and user defined type, and some advanced SQL. [51], [52], [53]

##### cons:
 1.  Replication solution is not as good as MySQL. [53]    

####  28   Microsoft Access        

##### pros:
 1.  Access is a file-server based database. Access is a part of Microsoft Office and used for building application. Access supports VBA and SQL can also be used in VBA. Access can import or export data fro Excel, XML, Oracle, MySQL and etc. [54]    

##### cons:
 1.  Access does not support triggers, stored procedures and transaction logging and cannot deal with a large amount of data. All data is stored in one file which destories scalability. Only supports up to 255 concurrent users. [54], [55] 

####  29   SQLite        

##### pros:
 1.  SQLite is a free, open source relational database management system. Supports ACID and most of SQL-92 standard. SQLite is popuar as an embeded database and is the built-in database system in Android and iPhone. Data type in SQLite is weak (specified to value instead of column) which increases flexibility. Two read operations can execute in parallel. Supports a large group of programming languages. Easy to setup, great for rapid development. [56], [58] 

##### cons:
 1.  SQLite can not write if there are any other accesses, therefore can not handle high concurrency well. SQLite doesn't support user administration control and its SQL syntax is unique. [56], [57], [58]

####  30   Solr        

##### pros:
 1.  Solr is an open source, highly scalable, hit highlighting, faceted search, dynamic clustering, database integration, rich document (Word, PDF) handling, full-text search platform based on Lucene written in Java. Supports distributed search (split shards), index replication, HTTP/XML REST interface, JSON API. [59], [60], [61]

##### cons:
 1.  Solr needs a schema. [60]    

####  31   FileMaker       

##### pros:
 1.  FileMaker is a relational database with GUI interface (supports drag and drop). Can be used in Windows, OS X, iOS. Provides built-in functions and supports user script to access the database with a script debugger (break point, step). Can install an ODBC driver to connect MySQL, SQL Server and Oracle and read, create, edit, delete the records. [62], [63] 

##### cons:
 1.  Lack of scalability, requires mouse to execute some operations. [63]    

####  32   Hive        

##### pros:
 1.  Hive is a data warehouse written in Java built on Hadoop used for large data analysis. Provides a SQL-like language (easy to transfer from SQL to Hive) called HiveQL which has schema and translates queries to map/reduce, Apache Tez and Spark jobs. Its metadata is stored in RDBMS which reduces time to perform query semantic check. Supports index (including compaction and bitmap index), different shortage type (text, RCFile, HBase, ORC and etc.), user defined functions. Amazon Elastic MapReduce is a fork project of Hive. [64], [65] 

##### cons:
 1.  Hive is good at querying, but not as flexible as Pig for data management. Reply on external database to store metadata which may raise security problem. [65]    

####  33   Informix        

##### pros:
 1.  Informix is used for OLTP with high tranction rate for dataset based on time series and spatial data. Supports object-relational model and therefore supports more data types than SQL standard. Supports heterogeneous clustering (which provides high levels of redundancy and fault tolerance). Offers free developer edition and an warehouse edition which is a column based database with in-memory data, tokenization, deep compression features. [66]    

####  34   Splunk        

##### pros:
 1.  Splunk is used for machine generated data (infrastructure, security system and busisness applications) anlysis with hundreds of apps to various machine/software generated data. Supports structured and unstructured machine generated data indexing. Supports real-time and historical search, reporting and statistical anlysis by using SPL (search processing language). Supports multi-site clustering, automatic load balancing, unlimited number of concurrent users, enterprise-wide administration, authenticated transaction. [67], [68]

##### cons:
 1.  Setup costs are expensive and complex. [69]    

####  35   SAP HANA        

##### pros:
 1.  SAP HANA is a column based, ACID compliant, in-memory databse used to process high volumes of data in real-time. [16], [17] 
 2.  Support SQL and MDX. [16]    
 3.  Has a programming component (embeded web server and versiion control repository) that allows customized application to run on it. [16]    

##### cons:
 1.  SAP HANA has a steep learning curve and is not so much suitable for non-SAP ERP users. [18]    

####  36   Firebird        

##### pros:
 1.  Firebird is an open source, cross platform, SQL relational database management system. Supports ACID, MVCC (writer does not block reader), stored procedures, triggers, cursor in PostgreSQL. Supports user defined functions, third party tools. Backups are incremental. Provides API for many programming languages. [70]    

##### cons:
 1.  Due to MVCC, maintenance is reuqired to clean up old versions of data. Firebird does not have administration control. [70], [71] 

####  37   MariaDB. [73]    

##### pros:
 1.  The community-developed fork of MySQL due to concern over close source risk of MySQL. Compared to MySQL, MariaDB has more storage engines, faster performance (group commit, pool of threads and etc.) and more features (subquery). [72], [73], [74]

####  38   Vertica Anlytics Platform       

##### pros:
 1.  Vertica Anlytics Platform is a column based analytic database management system with shared nothing architecture working on large, fast-growing volumes of data. Provides fast query performance for data warehouse and query-intensive applications. Supports standard SQL interface with many analytics functions, compression, automated data replication, server recovery, query and storage optimization. Provides free community edition. [75]    

####  39   Amazon DynamoDB       

##### pros:
 1.  Amazon DynamoDB is a key/value store and is a part of AWS. Has multi-master feature to deal with version conflict. Provides synchronous replication across different data centers. Data is stored in SSD in different servers and performance is scalable and predictable. Its charge is based on throughput instead of storage and the users don't need to care about the management of software and hardware. [76], [77] 

##### cons:
 1.  64KB limit on row size, 1 MB limit on querying. Good for looking up by keys, limited for queries, especially for queries on non-inedexed data Doesn't support changing index on the fly. Doesn't support secondary indexes, joins, ACID, triggers, server-side scripts. [77]    

####  40   dBASE       

##### pros:
 1.  dBase is first released in 1979 for microcomputers. dBase is an alternative for access or FileMaker. [78], [79] 

##### cons:
 1.  dBase only runs on Windows and is not scalable. [79]    

####  41   Sphinx        

##### pros:
 1.  Sphinx is a free, open source, distributed, scalable, full text (index document as keywords for quick search) search engine. Supports stand-alone server operation. Can be connected to other DBMS by native protocols (MySQL, MariaDB and PostgreSQL) or ODBC. Sphinx is fast since it directly connects to the database. Sphinx can be used as a storage engine for MySQL and MariaDB. Sphinx has schema, but also provides a JSON attributes for attributes that are not listed in the schema to improve flexibility. [80], [81] 

##### cons:
 1.  Doesn't support partial index update. [81]    

####  42   Ingres        

##### pros:
 1.  Ingres is an open source, SQL relational database management system. Supports ACID. [82], [83] 

####  43   MarkLogic       

##### pros:
 1.   MarkLogirc is a distributed, scalable, ACID compliant, document based (XML, JSON, RDF, and geospatial data) database. Can use HDFS directly. Suports multiple indexing, replication, rollback, automated failover, point-in-time recovery, backup/restore, backup to Amazon S3, parallelized ingest, role-based security, full text search, location services, geospatial alerting, RDF triple store and SPARQL query. [84]    

####  44   Ehcache       

##### pros:
 1.  Ehcache is an open source, distributed cache for performance boosting written in Java. Features memory and dist store, replicate by copy and invalidate, listeners, cache loaders, cache extensions, cache exception handlers, a gzip caching servlet filter, RESTfull and SOAP APIs. [85], [86] 

##### cons:
 1.  Ehcache was bought by Terracotta and some new features are only available in commercial edition. [85]    

####  45   RavenDB       

##### pros:
 1.  RavenDB is an open source, schema free, document based (JSON) databased for .NET. Use HTTP/JSON to get access to data. Supports sharding and replication, implicit or explicit indexing, powerful text search based on Lucene. [87], [88] 

##### cons:
 1.  Only for .NET. [87]    

####  46   Hazelcast       

##### pros:
 1.  Hazelcast is an in-memory, open source, synamic scalable data grid written in Java. Data is evenly stored in nodes from the same server. Backups are arranged in the same way to protect single node failure. Provides schema-less structure, REST API. Hazelcast can be used in front of a database for caching frequently used data into memory, storing temporal data (web sessions), in-memory data processing, cross JVM communication. [89], [90], [91]

##### cons:
 1.  In case of all nodes failure, the data will be lost. [92]    

####  47   InterBase       

##### pros:
 1.  InterBase is a corss platform relational database management system with small footprint (small disk and memory usage), little administration requirements and multi-generational architecture (MVCC). InterBase is SQL-92 compliant and supports JDBC, ODBC and  ADO.NET interfaces. InterBase also supports built-in encryption, rollback (which is based on multi-generational architecture and is near-instantaneous). [93]    

##### cons:
 1.  Due to multi-generational architecture, some operations are difficult to implement and relative slow compared to tranditional relational database. [93]    

####  48   SQL Anywhere        

##### pros:
 1.  SQL Anywhere, a.k.a Sybase SQL Anywhere, is a cross platform (it can run on different platforms and database file can be copied across different platforms) relational database management system. Provides interface for ODBC, JDBC,  ADO.NET, PHP and Perl. Supports stored procedure, user defined functions, triggers, referential integrity, row-level locking, replication and system or scheduled events. Provides high availability, proxy tables. [94]    

####  49   mSQL       

##### pros:
 1.  mSQL is a lightweight database management system. [95]    

##### cons:
 1.  It is surpassed by MySQL in popularity and becomes a less commonly used database. [95]    

####  50   HyperSQL       

##### pros:
 1.  HyperSQL is a lightweight, relational database management system written in Java. HyperSQL is a desktop database used for a single application. Supports a large portion of SQL-92 and SQL:2008 standards. Data is stored both in memory and in disk. User can get access to the database through a built-in web server, a GUI and commend line. HyperSQL can run in 3 modes to deal with concurrency control: table level locks, MVCC and a combination of locks and MVCC. [96], [98]    

##### cons:
 1.  HyperSQL is not very fast, especially for large tables. [97]  

####  51   ADABAS       

##### pros:
 1.  ADABAS is an inversed list database, first released in 1971 for IBM mainframe system. ADABAS is acronym for Adaptable Data Base System. ADABAS stores data in files and regards file as its organizational unit. Can search on indexed or non indexed fields (attributes). ADABAS is faster and more compressed than DB2. [99], [100]    

##### cons:
 1.  ADABAS doesn't have a SQL engine embeded. Can use ADABAS SQL gateway (provides OBDC, JDBC, OLE DB) to get access to the database. Doesn't support referential integrity. [99], [100]  

####  Reference:

[1] http://azure.microsoft.com/en-us/pricing/free-trial/   
[2] http://azure.microsoft.com/en-us/campaigns/azure-vs-aws/  
[3] http://azure.microsoft.com/en-us/services/sql-database/  
[4] http://www.databasejournal.com/sqletc/article.php/3869736/Choosing-a-Database-Platform.htm  
[5] https://en.wikipedia.org/wiki/Teradata  
[6] https://www.digitalocean.com/community/tutorials/a-comparison-of-nosql-database-management-systems-and-models  
[7] https://cwiki.apache.org/confluence/display/COUCHDB/Introduction  
[8] http://couchdb.apache.org/  
[9] http://www.tutorialspoint.com/mongodb/mongodb_advantages.htm  
[10]  http://www.mongodb.org/  
[11]  http://halls-of-valhalla.org/beta/articles/the-pros-and-cons-of-mongodb,45/  
[12]  http://stackoverflow.com/questions/5244437/pros-and-cons-of-mongodb  
[13]  http://kkovacs.eu/cassandra-vs-mongodb-vs-couchdb-vs-redis  
[14]  http://www.ehow.com/info_12172600_list-pros-cons-oracle-database-11g.html  
[15]  https://en.wikipedia.org/wiki/Sybase_IQ  
[16]  http://searchsap.techtarget.com/definition/HANA-SAP-HANA  
[17]  https://en.wikipedia.org/wiki/SAP_HANA  
[18]  https://www.trustradius.com/reviews/sap-hana-2014-06-09-09-41-33  
[19]  https://en.wikipedia.org/wiki/Memcached  
[20]  https://en.wikipedia.org/wiki/Redis  
[21]  http://www.bigdatalittlegeek.com/blog/2014/3/25/memcached-vs-redis  
[22]  http://database.ittoolbox.com/groups/vendor-selection/dbms-select/oracle-11g-vs-sybase-iq-1882882  
[23]  https://en.wikipedia.org/wiki/MySQL_Cluster  
[24]  http://stackoverflow.com/questions/5300490/mysql-cluster-ndb-vs-mysql-replication-innodb-for-rails-3-apps-pros-cons  
[25]  http://www.smartfile.com/blog/the-pros-and-cons-of-mysql/  
[26]  https://en.wikipedia.org/wiki/MySQL  
[27]  https://en.wikipedia.org/wiki/IBM_DB2  
[28]  http://www.ehow.com/info_12106599_advantages-db2.html  
[29]  https://en.wikipedia.org/wiki/Riak  
[30]  https://blog.mozilla.org/data/2010/05/18/riak-and-cassandra-and-hbase-oh-my/  
[31]  https://en.wikipedia.org/wiki/Apache_Cassandra  
[32]  https://en.wikipedia.org/wiki/OrientDB  
[33]  https://en.wikipedia.org/wiki/Draft:ArangoDB  
[34]  https://en.wikipedia.org/wiki/Neo4j  
[35]  https://news.ycombinator.com/item?id=7246849  
[36]  https://groups.google.com/forum/#!topic/neo4j/mts6H9Py-2I  
[37]  https://en.wikipedia.org/wiki/Elasticsearch  
[38]  https://en.wikipedia.org/wiki/Apache_Accumulo  
[39]  http://accumulo.apache.org/1.4/user_manual/Security.html  
[40]  https://karussell.wordpress.com/2011/07/13/jetslide-uses-elasticsearch-as-database/  
[41]  http://apache-accumulo.1065345.n5.nabble.com/How-does-Accumulo-compare-to-HBase-td10464.html  
[42]  https://code.google.com/p/scalaris/  
[43]  http://scalaris.googlecode.com/svn/trunk/user-dev-guide/main.pdf  
[44]  https://en.wikipedia.org/wiki/VoltDB  
[45]  http://voltdb.com/fast-smart-scale  
[46]  http://highscalability.com/blog/2010/6/28/voltdb-decapitates-six-sql-urban-myths-and-delivers-internet.html  
[47]  https://en.wikipedia.org/wiki/Aerospike_database  
[48]  http://www.dbms2.com/2012/08/27/aerospike-the-former-citrusleaf/  
[49]  https://en.wikipedia.org/wiki/Tokyo_Cabinet_and_Kyoto_Cabinet  
[50]  http://fallabs.com/kyototycoon/  
[51]  https://en.wikipedia.org/wiki/PostgreSQL  
[52]  http://www.anchor.com.au/hosting/dedicated/mysql_vs_postgres#head-e1573b42fddb2f6189d92926583b54b2a4f3ef51  
[53]  http://www.quora.com/What-are-pros-and-cons-of-PostgreSQL-and-MySQL  
[54]  https://en.wikipedia.org/wiki/Microsoft_Access  
[55]  http://www.learnitanytime.com/4031/know-the-advantages-and-disadvantages-of-microsoft-access-2/  
[56]  https://en.wikipedia.org/wiki/SQLite  
[57]  https://www.digitalocean.com/community/tutorials/how-and-when-to-use-sqlite  
[58]  http://stackoverflow.com/questions/3630/sqlite-vs-mysql  
[59]  https://en.wikipedia.org/wiki/Apache_Solr  
[60]  http://www.ymc.ch/en/why-we-chose-solr-4-0-instead-of-elasticsearch  
[61]  http://www.quora.com/What-are-the-pros-and-cons-of-Woosh-vs-Solr-vs-ElasticSearch  
[62]  https://en.wikipedia.org/wiki/FileMaker  
[63]  http://stackoverflow.com/questions/421960/what-are-the-pros-and-cons-of-filemaker  
[64]  http://en.wikipedia.org/wiki/Apache_Hive  
[65]  http://www.quora.com/What-are-the-pros-and-cons-between-Pig-and-Hive  
[66]  http://en.wikipedia.org/wiki/IBM_Informix  
[67]  http://en.wikipedia.org/wiki/Splunk  
[68]  https://www.splunk.com/en_us/products/splunk-enterprise.html  
[69]  http://www.itcentralstation.com/product_reviews/splunk-review-by-tal-weiss  
[70]  http://en.wikipedia.org/wiki/Firebird_%28database_server%29  
[71]  http://stackoverflow.com/questions/2964379/migrating-from-sql-server-to-firebird-pro-and-cons  
[72]  http://en.wikipedia.org/wiki/MariaDB  
[73]  https://mariadb.com/kb/en/mariadb/mariadb-vs-mysql-features/  
[74]  http://news.dice.com/2013/05/22/mariadb-vs-mysql-a-comparison-2/  
[75]  http://en.wikipedia.org/wiki/Vertica  
[76]  https://en.wikipedia.org/wiki/Amazon_DynamoDB  
[77]  http://www.slideshare.net/saniyakhalsa/dynamo-db-pros-and-cons  
[78]  https://en.wikipedia.org/wiki/Dbase  
[79]  http://www.linuxquestions.org/questions/programming-9/review-dbase-what-do-you-think-854312/  
[80]  https://en.wikipedia.org/wiki/Sphinx_(search_engine)  
[81]  http://stackoverflow.com/questions/737275/comparison-of-full-text-search-engine-lucene-sphinx-postgresql-mysql  
[82]  https://en.wikipedia.org/wiki/Ingres_(database)  
[83]  https://www.princeton.edu/~achaney/tmve/wiki100k/docs/Ingres_(database).html  
[84]  https://en.wikipedia.org/wiki/MarkLogic  
[85]  https://en.wikipedia.org/wiki/Ehcache  
[86]  http://www.ehcache.org/about  
[87]  http://www.codeproject.com/Articles/74322/RavenDB-An-Introduction  
[88]  http://www.slideshare.net/goldshtn/introduction-to-ravendb  
[89]  https://en.wikipedia.org/wiki/Hazelcast  
[90]  http://hazelcast.com/products/hazelcast/  
[91]  http://www.quora.com/How-does-Redis-compare-to-Hazelcast-What-are-the-pros-and-cons-of-using-either-of-them  
[92]  http://mikepilone.blogspot.com/2013/01/hazelcast-jms-provider.html  
[93]  https://en.wikipedia.org/wiki/InterBase  
[94]  https://en.wikipedia.org/wiki/SQL_Anywhere  
[95]  https://en.wikipedia.org/wiki/MSQL  
[96]  https://en.wikipedia.org/wiki/HSQLDB  
[97]  http://www.yellowfinbi.com/YFForum-Should-I-use-HSQL-or-another-DBMS-like-SQLserver-?thread=99961  
[98]  https://forum.openoffice.org/en/forum/viewtopic.php?f=40&t=20736  
[99]  https://en.wikipedia.org/wiki/ADABAS  
[100] http://tech.forums.softwareag.com/techjforum/posts/list/21734.page  
[101] https://en.wikipedia.org/wiki/Couchbase_Server
