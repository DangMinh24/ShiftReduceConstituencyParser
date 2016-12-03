# ShiftReduceConstituencyParser


Trivial attempt of re-coding Shift-Reduce Parser for Constituency Grammar.

After reading paper [Yue Zhang] Fast and Accurate Shift-Reduce Constituent Parsing :http://www.aclweb.org/anthology/P13-1043.pdf

Pratice is a best way to see how much yourselves understand about problem.

Shift-Reduce Parsing uses 2 items: stack S, and queue W, where W is place to hold all words need to be parsed. Shift-reduce working depends on these actions: Shift, Reduce Unary, Reduce Binary, Terminate. However, these actions usually be chosen appropriately depend on the current state of both S and W. However, people try to make a classifier that can predict which actions should be used in each state. 

The idea of the paper is : Manually parse each sentence. At each steps when parsing a sentence, they try to read and extract feature value, corresponding with an appropriate action. So we can get feature set X and set of labels y. The problem now is experiment which different models to choose the best one for this "mutil-label problem"
