# 516homework
				Comparison Type 
1	MongoDB 		
	Intro				Non-relational		
						as-a-Service	
		Pros		Availability	High availability with replica sets. 				  								
				Flexibility	Offers flexible schema structuring data into JSON which has a more natural data 						format and richer data structure.
						Transitioning from Relational Databases to MongoDB - Data Models
		Cons				The default setup was vulnerable to client crashes, limitations of MongoDB when 						used on 32-bit systems. In some cases, this is due to the inherent memory 							limitaion 	
						Lack of traditional RDBMS features: 	3
		Reference 			http://docs.mongodb.org/manual/core/replication-introduction
						http://blog.mongodb.org/post/137788967/32-bit-limitations
2	CouchDB 						
				
			Cons			Lack of sophisticated declarative query language
						Lack of native query processing constructs	
						Transaction management providing ACID safety guarantees	
						Couch maintains a different document for every update you make. This is done to 						save all revisions of a document. Although this is a positive feature, this 							fills up your hard disk fast. You can run asynchronous compaction to delete 							all old revisions, but 	this generally takes hours and is system intensive	
		Reference			"Enabling JSON Document Stores in Relational Systems" by Craig Chasseur. 							University Of 	Wisconsin chasseur@cs.wisc.edu. Yinan Li. University Of 							Wisconsin.
3	MySQL		Intro			BigTables		
						General purpose		
						MySQL ecosystem		
						Key value direct access		
						Relational		
			Pros			MySQL has the biggest market share of any open source database.		
						Full-text indexing and searching		
			Cons			MySQL does not currently comply with the full SQL standard for some of the 							implemented functionality, including foreign key references when using some 							storage engines other than the default of InnoDB										Triggers are limited to one per action / timing,		
						Is strongly limited by hard disk performance. (This is a common drawback for 							transactional relational database)		
			Reference		http://dev.mysql.com/doc/refman/5.6/en/innodb-foreign-key-constraints.html
4	MariaDB						
			Intro			A community-developed fork of the MySQL relational database management system 							intended to remain free under the GNU GPL.		
			Pros			Supports Ruby								
						Can Develop in Both Iphone and Android (Objective C and Java, plus others)
						Open Source, Non-Propreity		
			Cons			Cannot develop in wide range of evo languages like Actionscript, Delphi, 							PowerShell and JavaScript		
						Does not support OS X platform for Iphone and Amazon Cloud MapReduce, which 							MongoDB does	
			Reference 		https://ahsannabi.wordpress.com/swot-analysts-mariadb-or-mongodb/
5	Google App Engine	
			Intro			Big Tables					
			Pros			It provides more infrastructure to make it easy to write scalable applications, 						but can only run a limited range of applications designed for that								infrastructure.	All billed High-Replication Datastore App Engine applications 						have a 99.95% uptime SLA(Service-level agreement)	
						All billed High-Replication Datastore App Engine applications have a 99.95% 							uptime SLA
						Sustain multiple datacenter outages without any downtime.	
			Reference		"Google App Engine Blog: Happy Birthday High Replication Datastore: 1 year, 							100,000 apps, 0% downtime". Googleappengine.blogspot.com. 2012-01-05. 								Retrieved 2012-02-14.
			Cons			Users may upload arbitrary Python modules, but only if they are pure-Python; C 						and Pyrex modules are not supported.	
			Reference	
						Datastore cannot use inequality filters on more than one entity property per 							query
						Developers have read-only access to the filesystem on App Engine. Applications 						can use only virtual filesystems, like gae-filestore.	
						Does not support sticky sessions (a.k.a. session affinity), only replicated 							sessions are supported including limitation of the amount of data being 							serialized and time for session serialization.	
			Reference		https://cloud.google.com/appengine/docs/python/?csw=1#Quotas_and_Limits
						"Google App Engine Datastore Gotchas « aleatory". Aleatory.clientsideweb.net. 							2009-11-28. Retrieved 2012-02-14.
						"gae-filestore - Simple Virtual File System on Google App Engine DataStore - 							Google 	Project Hosting". Code.google.com. Retrieved 2012-02-14.
						"A process started on the server to answer a request can't last more than 60 							seconds (with the 1.4.0 release, this restriction does not apply to background 						jobs anymore).
					
6	Google Cloud Datastore	
			Intro 			Big Tables					
			Pros			Scalable datastore	
						Google Cloud Datastore is a fully managed, schemaless database for storing non-						 	relational data. Cloud Datastore automatically scales with your users and 							supports ACID transactions, high availability of reads and writes, strong 							consistency for reads and ancestor queries, and eventual consistency for all 						other queries. 	
						https://cloud.google.com/datastore/docs
				Fully Managed	Each Cloud Datastore instance is fully managed by Google so there is no planned 						downtime, replication across multiple datacenters, automatic scaling as your 							traffic increases, and monitoring by Google Engineers. 		
				Flexibility	Cloud Datastore is accessible via HTTP using a JSON or Protocol Buffers API, 							running on top of the Google APIs infrastructure. Cloud Datastore offers 							Protocol Buffer client libraries for Java and Python as well as support for 							the Google APIs client libraries. In addition, Cloud Datastore offers a 							web-based interface for managing your Cloud Datastore instances, and a 								development server to support local development.		
7	"Sqrrl Enterprise"						
			Pros			Operational data store for large amounts of structured and unstructured data
						It is the only NoSQL solution that scales elastically to tens of petabytes of 							data and has fine-grained security controls.	
						Enables development of real-time applications on top of Big Data	
						Sqrrl uses HDFS for storage; Accumulo for security/speed of access; Thrift API 						for interactivity; and works with map/reduce, visualizations, third party software, 							and existing schema explored databases.	
						Sqrrl Enterprise excels in use cases such as advanced data breach detection, 							fraud/waste/abuse analysis, and intelligence 											processing/exploitation/dissemination	
			Cons	Ease-of -use	Sqrrl simplifies the use of Accumulo with installation tools, data loading 							tools, and world-class support from the creators of Accumulo.	
				Search&Query	Sqrrl improves this API by adding richer search and query capabilities, 							including full-text keyword search, document search (i.e., JSON document 							support), a SQL-like queries, and graph search.	
				Security	Sqrrl extends this cell-level security capability with a labeling engine that 							automates application of the security labels, a policy engine that supports 							Role-Based and Attribute-Based Access Controls, encryption-at-rest and 								encryption-in-motion, and auditing capabilities		
8	Affinity		Pros		Flexible Communication Channels:Representing any communication channel with a							PIN,accessing channels via one simple uniform syntax
				
						Mobile Ad-Hoc Networks:Use of mDNS, its support for FSMs		
						Extendable Service Libraries:Be it for platform-dependent considerations, 							performance, portability or any other reason, the kernel's service 								infrastructure and compact service interface make it easy to integrate 								lower-level programming languages 		
						Easy Data Transformations		
						Everything in AffinitiNG is stored as a PIN, meaning that everything can be 							queried, correllated, joined		
						In Affinity, each instance of an entity (aka PIN or object or instance) is free 						to contain any attribute at any time. 
				Reference 	http://affinityng.cfapps.io/doc/strengths.html
9	AllegroGraph		Pros		Completely multi-processing based (SMP) – Automatic Resource Management for all 						processors and disks, and optimized memory use.		

						Efficient memory utilization in combination with disk-based storage	
						Supports SPARQL, RDFS++, and Prolog reasoning from numerous client 								applications.		
						Full and Fast Recoverability		
						Advanced Text Indexing 		
						Dynamic and Automatic Indexing 		
						Column-based compression of indices
			Reference		http://franz.com/agraph/allegrograph/
10	Antibase HDB		
			Intro			In-Memory database with hybrid architecture		
			Pros			Provide real time ACID properties and full standard SQL whereas NoSQL does not 						support those features.		
							
11	ALTIBASE XDB	
			Intro				
			Pros			ALTIBASE XDB (Extreme In-Memory Database) is the world’s fastest In-Memory only 						database.								
						ALTIBASE XDB maximizes In-Memory database capabilities to be the fastest 							database with  direct attach mode (DCI mode) to eliminate overhead. 	
						Provide real time ACID properties and full standard SQL whereas NoSQL does not 						support those features.		
			Cons	NoSQL weakness	NoSQL is not a relational database and does not support standard API. 	
						NoSQL is not designed to store structured data and is prone to data 								NoSQL is not suitable for complicated operations such as UPDATE.	
						It is difficult to prevent data duplication with NoSQL. 	
						It is complicated to back up and recover data with NoSQL	
						NoSQL is not suitable for ad-hoc query and analysis.	
						NoSQL has low product maturity and is not stable and reliable.	
						It is difficult to install and maintain NoSQL.	
						There is inadequate support for NoSQL users.	
						There are few experts available specialized in NoSQL.							Reference	 http://altibase.com/in-memory-database-hybrid-products/xdb/#sthash.Y9Ok0f8u.dpuf
	
12	ActiveSpaces		
			Intro		In-memory, For Java/.Net./C, distributed, hybrid, event enabled, NewSQL		
			Pros	General Pros for In memory database	
						Main memory databases are faster than disk-optimized databases since the 							internal optimization algorithms are simpler and execute fewer CPU 								instructions. Accessing data in memory eliminates seek time when querying the 						data, which provides faster and more predictable performance than disk.		
13	Oracle Database	Hadoop					
			Pros			Available on multiple platforms such as Windows, all flavors of Unix from 							vendors such as IBM, Sun, Digital, HP, Sequent, etc. and VAX-VMS, as well as 							MVS. The multi-platform nature of Oracle makes it a true enterprise solution.
			
						Dynamically re-create a read-consistent image for a reader of any requested 							data that has been changed but not yet committed. In other words, the reader 							will see the data as it was before the writer began changing it (until the 							writer commits)	
						
						Oracle has major advantages in terms of locking and concurrency.	
			Reference	http://searchoracle.techtarget.com/tip/Oracle-vs-SQL-Server-Why-Oracle-wins		
14	Microsoft SQL Server	
			Intro 			Hadoop					
			Pros			SQL Server is SAP-certified to run some of the most demanding workloads. Ge 							more predictable performance of virtualized SQL Server instances with IO 							governance in Resource Governor.	
			
						Availability &disaster recovery	Gain greater uptime, faster failover, improved 						manageability, and better use of hardware resources through AlwaysOn, a unified 							solution for high availability.	
						
			Security 		Transparent data encryption, robust auditing, extensible key management and 							encrypted backups. It is even easier to manage permissions for data access to 						support separation of duties across various users.
			
			In-memory performance	With SQL Server 2014, new in-memory capabilities for transaction processing and 						enhancements for data warehousing complement our existing technologies for data 						warehousing and analytics. 		
			
			Cons			No multi-version consistency model, which means that "writers block readers and 						readers block writers" to ensure data integrity.	
						SQL Server's locking scheme is much simpler (less mature) and will result in a 						lot of delays/waits in a heavy OLTP environment.
			Reference				http://www.microsoft.com/en-us/server-cloud/products/sql-server/default.aspx?WT.srch=1&WT.mc_id=Unsassigned_GOO_USEvergreenSearch_Unassigned&CR_CC=Unassigned
			
15	ArangoDB 	Graph					
			Pros	Reduce duplication
						Have a consistent HTTP API for  different services or applications and don’t 							duplicate logic between them.		
						
						Reduce the number of requests between database and backend
						
						Abstractions over implementation details
						
						Execute data intensive operation
						
						API for your mobile or single page web applications
						
				Reference	https://www.arangodb.com/foxx
							
16	PostgreSQL	Based on the object relational DBMS Postgres					
			Pros	Flexibility	New JSONB data type for PostgreSQLsupports fast lookups and simple expression 							search queries using Generalized Inverted Indexes (GIN).Allowing user to have 						relational and non-relational data stores at the same time		
				Replication system
						Logical decoding supplies a new API which allows reading, filtering, and 							manipulating the replication system. The new API is the base for new 								replication tools, such as bi-directional replication, which supports the 							creation of multi-master PostgreSQL clusters. Other improvements to the 							replications also include replication slots and time delayed replicas.		
18	Cassandra	Wide-column store based on ideas of BigTable and DynamoDB					
			Pros	Wide column Stores	
						Wide column stores, also called extensible record stores, store data in records 						with an ability to hold very large numbers of dynamic columns. Since the column 						names as well as the record keys are not fixed, and since a record can have 							billions of columns, wide column stores can be seen as two-dimensional 								key-value stores.
				Availabillity	No single point of failure ensures 100% availability.		
				Simplicity	Operational simplicity for lowest total cost of ownership.		
				Scalability	Best-in-class scalability of NoSQL platforms.		
			Cons			no JOINs, no aggregate functions	
			Reference		http://db-engines.com/en/article/Wide+Column+Stores
						http://db-engines.com/en/system/Cassandra
					
19	SQLite		Pros	Atomic 		Transactions are atomic, consistent, isolated, and durable (ACID) even after 							system crashes and power failures.

				Zero-configuration No setup or administration needed.		
				Cross-platform	Unix (Linux, Mac OS-X, Android, iOS) and Windows (Win32, WinCE, WinRT) are 							supported out of the box. Easy to port to other systems.		
						Comes with a standalone command-line interface (CLI) client that can be used to 						administer SQLite databases.		
			Cons			Has limited ALTER TABLE support, as it can't modify or delete columns.	26							 
						Partial support for triggers, and it can't write to views (however it supports 						INSTEAD OF triggers that provide this functionality)		
				Client/Server Applications	
						Weak performance when many client programs accessing a common database over a 							network. Should avoid using SQLite when same database will be accessed 								simultaneously from many computers over a network filesystem.		
						Splitting the database component off onto a separate machine, then you should 							definitely consider using an enterprise-class client/server database engine 							instead of SQLite.		
				Concurrency	SQLite supports an unlimited number of simultaneous readers, but it will only 							allow one writer at any instant in time. 		
				Large datasets	An SQLite database is limited in size to 140 terabytes (247 bytes, 128 								tibibytes). And even if it could handle larger databases, SQLite stores the 							entire database in a single disk file and many filesystems limit the maximum 						size of files to something less than this.
				Reference	http://sqlite.org/features.html
						"SQL Features That SQLite Does Not Implement". SQLite. January 1, 2009. 							Retrieved October 14, 2009.
20	Accumulo						
			Pros	Wide column Stores			
21	Hbase		
			Intro			Wide-column store based on Apache Hadoop and on concepts of BigTable					
			Pros	Wide column Stores	
				Consistency	Because it can utilize the storage, memory, and CPU resources of any number of 						servers, as well as has scale-out features like automatic sharding, HBase can scale 							limitlessly as load and performance demands increase simply by adding server 						nodes. HBase was designed from the ground up to provide optimal performance when 							consistency is critical.	
			Reference				http://www.infoworld.com/article/2848722/nosql/mongodb-cassandra-hbase-three-nosql-databases-to-watch.html
							
22	Redis	Key-value Stores					
			Pros	Speed		Redis holds its database entirely in memory, using the disk only for 								persistenc.Quickly update complex data structures like sorted sets or 								individual hash elements, and logs updates to disk sequentially for robust, 							low-overhead persistence (as long as you don't need to restart often).	
						Many key-value data stores have a limited set of datatypes, but Redis is 							comparatively rich, allowing for lists and sets of strings to be stored, as 							well as sorted sets and hashes. 		
						Redis can replicate data to any number of slaves.		
						Server can manipulate data directly		
						Used as a very fast cache for use cases where responsiveness is crucial	
			Cons			The size of the Redis datastore is limited to the size of the available 							memory		
					 	Requires consideration of data size to configure well
					 	Master-slave architecture means if the master wipes out, and SENTINEL doesn't 							work, the system is dead		
						
23	Lucene/Solr 	Intro			A widely used enterprise search engine based on Apache Lucene		
			Pros	Search Engines	Support for complex search expressions	27	
						Full text search		
						Stemming (reducing inflected words to their stem)		
						Ranking and grouping of search results		
						Geospatial search		
						Distributed search for high scalability	
			Reference		http://db-engines.com/en/article/Search+Engines
25	Splunk	Search Engine					
			Pros			Support for complex search expressions	27	
						Full text search		
						Stemming (reducing inflected words to their stem)		
						Ranking and grouping of search results		
						Geospatial search		
						Distributed search for high scalability	
			Reference		http://db-engines.com/en/article/Search+Engines	
26	MarkLogic	Search Engine					
			Pros			Support for complex search expressions	27	
						Full text search		
						Stemming (reducing inflected words to their stem)		
						Ranking and grouping of search results		
						Geospatial search		
						Distributed search for high scalability	
			Reference		http://db-engines.com/en/article/Search+Engines		
27	Teradata 	DBMS mainly used for data warehousing					
			Pros	Architecture	Teradata uses a massively parallel processing architecture with virtualized 							CPU, memory and storage that work together as a unit. With the Teradata Data 							Warehouse Appliance’s query optimizer and automated management of physical 							disk space, tuning measures are minimal. These features make the appliance 							easy to manage, which frees up database administrator resources for other tasks.	
				Performance	Teradata announced 700-times performance response time improvements from 							real-world deployments of the Teradata Data Warehouse Appliance 2750 that uses 						the Teradata Intelligent Memory and the latest Teradata Database.		
				Database Management
						Row-oriented and offer structures to enhance this orientation for analytics. 							Also provides columnar option, allowing queries to operate against row- and 							column-oriented data. Teradata Columnar offers true hybrid row and columnar 							capabilities that drastically improve query performance and deliver maximum 						data compression. 		
				Continuity, Upgrade and Expansion
						The Teradata Database is used on all Teradata platforms, so continuity, upgrade 						and expansion are available. The database fully supports business growth and 							data warehouse maturation by delivering efficient, predictable performance 							along with storage increases for system expansion or replacement.  								
						Teradata has its BYNET V5 communications stacked to run on top of the 40 							gigabytes per second InfiniBand.		
				 		
				 		Bi-directional Hadoop solution	Teradata offers a bi-directional Apache™ 							Hadoop® solution called SQL-H™ that allows developers to write standard SQL 							queries with extensions for Hadoop. It runs on all Teradata platforms. 								Besides providing access to Hadoop data, it can be a good strategy for 								storing multi-structured data.
				 		
			Reference		http://www.teradatamagazine.com/v14n01/Viewpoints/Face-Off/
28	Apache Hive	Data warehouse 		Software for querying and managing large distributed datasets, built on Hadoop					
29	IBM Informix						
			Pros			Hybrid database system that is capable of supporting relational and 								non-relational data		
						Informix 12.1 is the only database that allows different hardware and operating 						systems from cluster to cluster in a distributed environment. 		
				Real-time Analytics	
						Power OLTP and OLAP workloads and successfully meet service-level agreements 							(SLAs) for each		
				Fast, Always-on Transactions	
						Sets of options for keeping data available at all times, including zero 							downtime for maintenance		
				Sensor data management	
						Solves the big data challenge of sensor data with unmatched performance and 							scalability for managing time series data		
				NoSQL capability	
						Unleashes new capabilities, giving you a way to combine unstructured and 							structured data in a smart way, bringing NoSQL to your SQL database.	
30	Memcached Cloud 	
			Intro			In-memory key-value	
			Major 	Users
				LiveJourn,Wikipedia,Flickr,Bebo,Twitter,Typepad,Yellowbot,Youtube,WordPress.com,Craigslist,Mixi		
			Pros	Free & open source		
						Its API is available for most popular languages.		
						Caching small and static data	Memcached's internal memory managemen is more 							efficient because Memcached will consume comparatively less memory resources 							for metadata. Which are the only data type that are supported by Memcached, 							are ideal for storing data that's only 	being read because strings require 							no further processing. 		
				Horizontal scaling	
						Due in part to its design and in part to its simpler capabilities, 								Memcached is much easier to scale.		
			Cons			Doesn't do anything besides be an in-memory key/value store						Reference		http://www.bigdatalittlegeek.com/blog/2014/3/25/memcached-vs-redis
						Caches sharded by client do not scale across AWS zones		
						Adding a member to the pool requires reconfiguring and rebooting the client
						Unbalanced memcached clusters require a full system restart		
