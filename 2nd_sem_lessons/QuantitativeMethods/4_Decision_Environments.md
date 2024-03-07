###### Maximax Strategy
- *"Best of the Best"*
- It involves *looking at the best that could happen* for each possible course of action and then *choosing/selecting the action with the largest value*.

###### Maximin Strategy
- *"Best of the Worst"*
- It involves *looking at the worst that could happen* for each possible course of action and then *choosing/selecting the action with the largest value*

###### Minimax Strategy
- It involves *computing an opportunistic loss* `(or regret)` of each alternative by simply `subtracting the entry from that of the highest column value` and *selecting the maximum regret value of each row.* Finally, determine the decision by `choosing the minimum/lowest regret`.

###### Laplace Strategy
- It involves `calculating the average of each alternative` and then *choosing/selecting the alternative with the largest average*.

###### Hurwicz Strategy
- It involves `multiplying the best outcome in the row by the given vvalue of` *a*, and `adding the two result together`.

##### Formula
**EV** `=` **P**`(X)`, where
	**EV** `=` *expected value*
	**P** `=` *probability of an event*
	**X** `=` *amount to be received for a particular event*

Sample Problem:

Using *decision-making* under the condition of risk, find out *what alternative should be chosen*, considering the table that shows the assessed probability on each state of nature.