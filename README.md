# Decision Analysis 2021
The project focuses on analyzing decision alternatives using the payoff table. It has two conditions: under uncertainty "without probabilities" (by applying the three approaches: optimistic, pessimistic and regret) in case of revenues or costs and under risk "with probabilities" (by calculating the EVUR and EVUC to get the EVPI). The project is done using the C# language. 
## Decision alternatives with probabilities:
First, we compute the EVUR "Expected Value Under Risk" by multiplying each alternative by the probability of the decision and select the maximum value (in case of revenue) and the minimum (in case of cost)
Second, we compute the EVUC "Expected Value Under Certainty" by multiplying the maximum value in each column (in case of revenue) by its probability or the minimum value in each column (in case of cost) by its probability.
Finally, we get the absolute difference between EVUR and EVUC which will be referred to as EVPI "Expected Value for Perfect Information".
## Decision alternatives without probabilities:
*1. In the case of Revenue*
- Optimistic approach (Maximax): We get the maximum value of each row and select the maximum of them.
- Pessimistic "Conservative" approach (Maximin): We get the minimum value of each row and select the maximum of them.
- Regret approach (Minimax): First, we select the maximum of every column. Then, we create a table in which each value is subtracted from the maximum of the column where it exists. Finally, from this new table, we get the maximum value of each row and select the minimum of them.

*2. In the case of Cost*
- Optimistic approach (Minimin): We get the minimum value of each row and select the minimum of them.
- Pessimistic "Conservative" approach (Minimax): We get the maximum value of each row and select the minimum of them.
- Regret approach (Minimax): First, we select the minimum of every column. Then, we create a table in which each value is subtracted from the maximum of the column where it exists. Finally, from this new table, we get the maximum value of each row and select the minimum of them.
