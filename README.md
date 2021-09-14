# Real-SQL-Interview-questions
While preparing for Product/Data Analyst interviews, I couldn't find any real SQL queries that are asked, so here it is.

I will keep adding the questions here and link the solutions in the repository.

## 1. Product Analyst interview

1. Get the day wise D1 and D7 retention rate for last 30 days for a given date

Table available: App_opened

date | user_id
----- | ------
01-02 |  a
01-02 | b
02-02 | c
.. |
.. |


Output:

date    |   D1   | D7
------- | ------ | -----
18-07(D0) |  50% |  30%
19-07(D0) | 40%  | 20%
...       |       |
...       |       |
18-08     |  40%  | -


2. Get comparison data as to how many people who opened the app, also searched and watched reels.
 
Tables available: 

App_opened table

date   |    user_id  
------ | ---------
01-02    |    a
01-02    |   b
02-02    |   c
..      |

search_open table

date    |   user_id  
------- | ----------
01-02   |     a
01-02   |    b
02-02   |    c
...     |

Reels_open

date    |   user_id     
-----   | -------
01-02   |    a
01-02   |    b
02-02   |    c
...     |


Output-

date     |   AO_to_RO   |    AO_to_SO    |     SO_to_RO
------  | ------------ | -------------   | ------------
18-07      |  50%         |    30%        |      15%
19-07      |  40%         |    20%        |      16%
...         |

