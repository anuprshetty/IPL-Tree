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

## Future Improvements:

## What I Learnt?

## References:
[MySQL official website](https://www.mysql.com/)

## Author Info:
- [LinkedIn](https://www.linkedin.com/in/anuprshetty/)
- [HackerRank](https://www.hackerrank.com/anuprshetty)

[Back To The Top](#IPL-Tree)
