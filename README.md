# Numbers
Numbers are important for designing systems and I often see Engineers including me falter , so here is my cheat sheet



|  Known as         | In Bytes       | Ten Powers Header | Actual Number
--------------------| -------------  | ------------      |---------------   
| Thousand ( 2^10)          |     1KB        | 10 ^ 3            | 1 000                             
| 1 Million (2^20)           | 1MB            | 10 ^ 6            | 1 000 000 
1 Billion   (2^30)        | 1GB            | 10 ^ 9            | 1 000 000 000
1 Trillion  (2^40)        | 1TB            | 10 ^ 12           | 1 000 000 000 000 
1 Quadrillion (2^50)       | 1PB            | 10 ^ 15           | 1 000 000 000 000 000
1 Quintillion       |                 | 10 ^ 18           | 1 000 000 000 000 000 000
1 Sextillion        |                 | 10 ^ 21           | 1 000 000 000 000 000 000 000
1 Septillion        |                 | 10 ^ 24           | 1 000 000 000 000 000 000 000 000 



What Latency numbers should i Know ?

1) L1 Cache reference  = 0.5ns
2) L2 Cache reference = 7 ns
3) Main memory reference = 100 ns
4) Read 1MB sequentially from memory = 250 micro seconds
5) Read 1MB sequentially from N/w = 10 ms
6) Read 1MB sequentially from Disk = 30 ms
7) Round trip with the same data center = 500 micro seconds
8) Disk seek = 10 ms
9) Send Packet CA->Netherlands->CA = 150 ms

Object Sizes:
I use Java , so these numbers depend on the language and implementation

|Datatype|Size
---------|-----
boolean | 1 bit
byte |  8 bits
char ( unicode) |  16 bits
short | 16 bits
int |  32 bits
float | 32 bits
double| 32 bits
long | 64 bits
UUID | 128 bits


Databases: The idea is to understand how much storage does different databases support and the capacity limitations / constraints.
While estimating the storage requirements ,we should also consider the space a Database needs to run compression. For example for Cassandra its about 30%.

How much space does Cassandra take while it runs through compression / compaction? This is needed to estimate storage requirements

Type|Db|Storage|Connections|Requests|Compression Reqs|Comments|
----|--|-------|-----------|--------|----------------|--------|
Columnar DB| Cassandra||||30% space|
GraphDB     |Neo4j||
Document|MongoDB
SQL|MySQL||
   |Oracle||
   
Web / Application Servers:
Type|Server|Requests|Connections|
----|------|--------|-----------|
App|Tomcat|||

Queues/ Streams:

Broker|Requests|Throughput|
-----|---------|----------|
Kafka|||
ActiveMQ|||
SQS|||
