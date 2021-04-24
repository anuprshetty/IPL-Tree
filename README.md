# IPL Tree
**IPL Tree** is a relational database system which helps to store and retrieve ***Indian Premier League*** data.  
***Normalization techniques*** are applied on this relational database model to minimize the redundancy in the database tables.

## E-R Model:
**Entity-Relationship model** for IPL Tree database.
![Entity-Relationship model](https://github.com/anuprshetty/IPL-Tree/blob/main/images/ipl_tree_schema.PNG)

## Tools and Technologies:
- MySQL Server
- MySQL Workbench

## Database Setup:
- Install MySQL Server and MySQL Workbench.
- Open MySQL Workbench.
- Create new database named **ipl_tree**
- Import and execute **ipl_tree.sql** and **normalized_ipl_tree.sql** files in MySQL Workbench.
- Play with **ipl_tree** database.

## Project Explanation:
IPL Tree database contains 8 tables.
<!--- Use 2 SPACEs at the end of a line for line break(\n). -->
1. player  
![player](https://github.com/anuprshetty/IPL-Tree/blob/main/images/player_table.png)
3. team  
![team](https://github.com/anuprshetty/IPL-Tree/blob/main/images/team_table.png)
5. owner  
![owner](https://github.com/anuprshetty/IPL-Tree/blob/main/images/owner_table.png)
7. coach  
![coach](https://github.com/anuprshetty/IPL-Tree/blob/main/images/coach_table.png)
9. c_match (Current match)  
![c_match](https://github.com/anuprshetty/IPL-Tree/blob/main/images/c_match_table.png)
11. venue  
![venue](https://github.com/anuprshetty/IPL-Tree/blob/main/images/venue_table.png)
12. individual_score (A player's score in a perticular match)  
![individual_score](https://github.com/anuprshetty/IPL-Tree/blob/main/images/individual_score_table.png)
14. total_score (A player's total score in all the matches)  
![total_score](https://github.com/anuprshetty/IPL-Tree/blob/main/images/total_score_table.png)

## Normalization:
Normalization is the process of minimizing redundancy from a relation or set of relations in a database.

### First Normal Form (1NF):
*If the table is flat, i.e., no composite and multivalued attributes, then we say that the relation is in 1NF.*

**player** table contains a multivalued attribute **role**. So **player** table is not in 1NF.  
***Conversion of player table to 1NF:***  
![1NF Conversion](https://github.com/anuprshetty/IPL-Tree/blob/main/images/1nf_conversion.png)

### Second Normal Form (2NF):
*A relation R is in 2NF if and only if
- R is in 1NF
- There is no partial dependency of a non-prime attribute to any key of R*

**player_1nf** table has primary key **(p_id, role)**. But all the non-prime attributes of **player_1nf** table are partially dependent on **p_id**. So **player_1nf** table is not in 2NF.  
***Conversion of player_1nf table to 2NF:***  
![2NF Conversion](https://github.com/anuprshetty/IPL-Tree/blob/main/images/2nf_conversion.png)

### Third Normal Form (3NF):
*A relation R is in 3NF if and only if
- R is in 2NF
- In any functional dependency, there shouldn't be the case that a non-prime attribute is determinied(derived) by another non-prime attribute.*

In **player_p2nf** table, non-prime attributes **(age, nationality)** are derived by the non-prime attribure **player_name**. So **player_p2nf** table is not in 3NF.  
***Conversion of player_p2nf table to 3NF:***  
![3NF Conversion](https://github.com/anuprshetty/IPL-Tree/blob/main/images/3nf_conversion.png)

### Boyce-Codd Normal Form (BCNF):
*A relation R is in BCNF if and only if
- R is in 3NF
- Whenever a non-trivial functional dependency, X --> A holds in R, then X should be a superkey of R. i.e., Determinants of all non-trivial functional dependencies must be superkeys.*

Determinants of all the non-trivial functional dependencies in **player_p3nf** table are superkeys. So **player_p3nf** table is already in BCNF.  

## Future Improvements:
- **IPL Tree** database system can be integrated with a web service so that user can easily interact with IPL data using web user interface.

## What I Learnt?
- Hands-on experience of working with MySQL Server and MySQL Workbench.
- Designing efficient relational database model.
- Constraints of relational model such as domain, key, entity integrity and referential integrity constraints.
- Hands-on experience on SQL langauges such as DDL, DML.
- Functional dependencies and normalization techniques.
- Understanding the usage and importance of indexing, B trees and B+ Trees in relational database tables.

## References:
- [MySQL official website](https://www.mysql.com/)

## Author Info:
- [LinkedIn](https://www.linkedin.com/in/anuprshetty/)
- [HackerRank](https://www.hackerrank.com/anuprshetty)

[Back To The Top](#IPL-Tree)
