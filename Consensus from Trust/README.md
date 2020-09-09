# CourseraCrypto-ConsensusFromTrust
The assignment is to design and implement a distributed consensus algorithm given a graph of “trust” relationships between nodes. This is an alternative method of resisting sybil attacks and achieving consensus; it has the benefit of not “wasting” electricity like proof-of-work does.

Nodes in the network are either compliant or malicious. The objective is to write a CompliantNode class (which implements a provided Node interface) that defines the behavior of each of the compliant nodes. The network is a directed random graph, where each edge represents a trust relationship. For example, if there is an A → B edge, it means that Node B listens to transactions broadcast by node A. We say that B is A’s follower and A is B’s followee.

The graph of nodes will have the following parameters:

the pairwise connectivity probability of the random graph: e.g. {.1, .2, .3}

the probability that a node will be set to be malicious: e.g {.15, .30, .45}

the probability that each of the initial valid transactions will be communicated: e.g. {.01, .05, .10}

the number of rounds in the simulation e.g. {10, 20}


# How to run this code

Run the following commands (with the arguments in the last line selected from the options above):

git clone https://github.com/aclaussen1/CourseraCrypto-ConsensusFromTrust.git

javac Simulation.java

java Simulation .1 .15 .05 10


# Results from test cases on coursera

Tests for this assignment involve your submitted miner competing with a number of different types of malicious miners

Running test with parameters: numNodes = 100, p_graph = 0.1, p_malicious = 0.3, p_txDistribution = 0.01, numRounds = 10
On average 45 out of 72 of nodes reach consensus

Running test with parameters: numNodes = 100, p_graph = 0.1, p_malicious = 0.3, p_txDistribution = 0.05, numRounds = 10
On average 61 out of 72 of nodes reach consensus

Running test with parameters: numNodes = 100, p_graph = 0.1, p_malicious = 0.45, p_txDistribution = 0.01, numRounds = 10
On average 34 out of 58 of nodes reach consensus

Running test with parameters: numNodes = 100, p_graph = 0.1, p_malicious = 0.45, p_txDistribution = 0.05, numRounds = 10
On average 41 out of 58 of nodes reach consensus

Running test with parameters: numNodes = 100, p_graph = 0.2, p_malicious = 0.3, p_txDistribution = 0.01, numRounds = 10
On average 67 out of 76 of nodes reach consensus

Running test with parameters: numNodes = 100, p_graph = 0.2, p_malicious = 0.3, p_txDistribution = 0.05, numRounds = 10
On average 74 out of 76 of nodes reach consensus

Running test with parameters: numNodes = 100, p_graph = 0.2, p_malicious = 0.45, p_txDistribution = 0.01, numRounds = 10
On average 39 out of 54 of nodes reach consensus

Running test with parameters: numNodes = 100, p_graph = 0.2, p_malicious = 0.45, p_txDistribution = 0.05, numRounds = 10
On average 49 out of 54 of nodes reach consensus




