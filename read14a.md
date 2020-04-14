# read 14:
## Database Normalization:
a process used to organize a database into tables and columns.
*main idea with this is that a table should be about a specific topic and only supporting topics included*

By limiting a table to one purpose you reduce the number of duplicate data contained within your database. This eliminates some issues stemming from database modifications.

### Reasons for Database Normalization:
There are three main reasons:
1. The first is to minimize duplicate data,
2. minimize or avoid data modification issues
3. simplify queries

### Data Duplication
Duplicated information presents two problems::
1. It increases storage and decrease performance.
2. It becomes more difficult to maintain data changes.

### Definition of Database Normalization
There are three common forms of database normalization:
 1st, 2nd, and 3rd normal form. 
 They are also abbreviated as 1NF, 2NF, and 3NF respectively. 

 *There are several additional forms, such as BCNF*

 ## normalization forms:
1. First Normal Form – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.
2. Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.
3. Third Normal Form – the table is in second normal form and all of its columns are not transitively dependent on the primary key

