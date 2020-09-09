# CourseraCrypto-ConsensusFromTrust
The assignment is to design and implement a distributed consensus algorithm given a graph of “trust” relationships between nodes. This is an alternative method of resisting sybil attacks and achieving consensus; it has the benefit of not “wasting” electricity like proof-of-work does.

Nodes in the network are either compliant or malicious. The objective is to write a CompliantNode class (which implements a provided Node interface) that defines the behavior of each of the compliant nodes. The network is a directed random graph, where each edge represents a trust relationship. For example, if there is an A → B edge, it means that Node B listens to transactions broadcast by node A. We say that B is A’s follower and A is B’s followee.

The graph of nodes will have the following parameters:

the pairwise connectivity probability of the random graph: e.g. {.1, .2, .3}

the probability that a node will be set to be malicious: e.g {.15, .30, .45}

the probability that each of the initial valid transactions will be communicated: e.g. {.01, .05, .10}

the number of rounds in the simulation e.g. {10, 20}
