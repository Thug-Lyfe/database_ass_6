# database_ass_6

Q.1 at In [5]

| index name     | size        | index type  |
| ------------- |:------------:| -----:|
| idx_17102_url	| 16kb	| USING btree |
| idx_17102_primary	| 16kb	| USING btree |
| circuits_position_idx	| 8kb	| USING gist |

Q.2 at In [6]
- 184 races has an age less than 38

Q.3 at In [7]
- 10 calls
- execution time 4.534 ms
First thing is to join the necesary tables: results, races, circuits & drivers.
Then it filters by position and driver age
then output the headers stated at the start: date,	surname,	age in years,	track in milliseconds,	race name &	circuit name

Q.4 at In [8],[9],[11]
- 1 call
- execution time 0.149ms
This selects everything from one table instead of filtering through multiple, making it obviously faster...
It should be noted that the materialized view does not account for new data entries after creation. So in essence it is just a saved image of a query.
