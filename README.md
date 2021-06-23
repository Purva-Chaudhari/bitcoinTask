# bitcoinTask
The solution is a greedy approach on density (fees/weight)<br>
A dataframe is created with sorted decreasing density transactions (index 0 is highest density)<br>
If a child transaction with higher density appears before, it calls (or prints) all its parent transactions before <br>
<br>
Scope of optimization: I guess it can be optimized more using knapsack 0-1 dynamic programming in parts (while considering inclusion of child and parent transactions) (Could not play around more due to time constraints)

### Programing information
Language: Python<br>
Libraries used: Numpy and pandas<br>
Input: mempool.csv<br>
Ouput: block.txt

### Results obtained so far 
Total Weights :  3999036 (There are still 900 weights remaining which could add a bit to total fees)<br>
(According to current algorithm it considers a transaction of weight 2204 further which accounts to total weight of 4,001,240 and Total fees 5,726,087)<br>
Total Fees: 5724849<br>
Total Transactions: 2216
