# [Evolving Neural Networks through Augmenting Topologies](https://ieeexplore.ieee.org/document/6790655)

[NEAT][1] algorithm is introduced to me by a youtube video who developed [MarIO][2].

### Key points
- Past studies have shown NE to be faster and more efficient than reinforcement learning methods such as Adaptive Heuristic Critic and Q-Learning on single pole balancing and robot arm control
- Because NE searches for a behavior instead of a value function, it is effective in problems with
continuous and high-dimensional state spaces
- In addition, memory is easily represented through recurrent connections in neural networks, making NE a natural choice
for learning non-Markovian tasks
-  NEAT is also an important contribution to GAs because it shows how it is possible for evolution to both optimize and complexify solutions simultaneously, offering the possibility of evolving increasingly complex solutions over generations, and strengthening the analogy with biological evolution.
- We present a novel NE method called NeuroEvolution of Augmenting Topologies (NEAT) that is designed to take advantage of structure as a way of minimizing the dimensionality of the search space of connection weights.
- NEAT = Genetic Encoding + Tracking genes through Historical Markings + Protecting Innovation through Speciation + Min Dimensionality through incremental growth from minimal structure

### Conclusions
- The main conclusion is that NEAT is a powerful method for artificially evolving neural networks. 
- NEAT demonstrates that evolving topology along with weights can be made a major advantage. Experimental comparisons verify that such evolution is several times more efficient than the neuroevolution methods so far. 
- Ablation studies show that historical markings, protection of innovation through speciation, and incremental growth from minimal structure all work together to produce a system that is capable of evolving solutions of minimal complexity. 
- NEAT strengthens the analogy between GAs and natural evolution by both optimizing and complexifying solutions simultaneously.
- We believe that the capacity to complexify solutions over the course of evolution offers the possibility of continual competitive coevolution and evolution of combinations of experts in the future.

### My Notes
This paper seems to be a logical paper. Taking analogies from genetic algorithms and applying it to the NN framework. Its not a rule that this method always outperform others but logically this method makes sense. One advantage is you can keep track of mutations and generations as the optimization process go through.

[1]: https://pastebin.com/ZZmSNaHX
[2]: https://www.youtube.com/watch?v=qv6UVOQ0F44
