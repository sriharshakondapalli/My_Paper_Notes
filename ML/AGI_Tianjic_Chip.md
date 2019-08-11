# [Towards artificial general intelligence with hybrid Tianjic chip architecture][1]

## Key Points:

- Given current progress in machine learning and neuroscience, an AGI system should have at least the following features
  - support for vast and complex neural networks that can represent rich spatial, temporal and spatiotemporal relationships
  - support for hierarchical, multigranular and multidomain network topologies, but without being limited to a specialized network structure
  - support for a wide range of models, algorithms and coding schemes
  - support for the intertwined cooperation of multiple specialized neural networks that are designed for different tasks in parallel processing
- The biggest is that an Artificial Neural Network (ANN) processes information in precise multibit values, while an Spiking Neural Network (SNN) uses binary spike trains
- To implement both models on one platform, the spikes need to be represented as digital sequences (1 or 0) so that they are compatible with the ANN coding format of digital number.
- Several other key points also need to be considered carefully
  - an SNN operates in spatiotemporal domains, which requires the memorization of historical membrane-potential and spike patterns within a certain duration, while an ANN accumulates the weighted activations intermediately and refreshes the information every cycle
  - the computation of an SNN includes membrane-potential integration, threshold crossing and potential reset, which is driven by spike events. By contrast, an ANN is related mainly to dense multiply-and-accumulate (MAC) operations and activation transformations.
  - the processing of spike patterns in SNNs requires a bit-programmable memory and extra high-precision memories to store the membrane potential, firing threshold and refractory period, whereas an ANN needs only byte-wise memories for activation storage and transformation
- By compiling various neural network models in both domains, we were able to carry out a detailed comparison to align the model dataflow, with one-to-one correspondence, to relevant building blocks—namely axon, synapse, dendrite, soma and router 
- By combining the axon, synapse, dendrite and soma blocks, we designed a unified functional core (FCore)   
- The FCore can act as an ANN/SNN converter
- To support the parallel processing of large networks or multiple networks concurrently, our Tianjic chip adopts a many-core architecture with scattered localized memory for timely and seamless communication
- The chip consists of 156 FCores, containing approximately 40,000 neurons and 10 million synapses
- Fabricated using 28-nm processing technology, Tianjic occupies a die area of 3.8 × 3.8 mm^2
- With its distributed on-chip memory and decentralized many-core architecture, Tianjic provides an internal memory bandwidth of more than 610 gigabytes (GB) per second, and yields an effective peak performance of 1.28 tera operations per second (TOPS) per watt in ANN mode when running at 300 MHz. 
- In SNN mode, synaptic operations are usually used to bench the chips, and Tianjic achieves an effective peak performance of about 650 giga synaptic operations per second (GSOPS) per watt
- We also developed a software tool that converts the multimodal and hybrid networks to meet the hardware constraints of the Tianjic chip automatically
- In general, Tianjic adopts a non-von Neumann paradigm with hybrid compatibility, many-core architecture, localized memory and streamlined dataflow, which is able to support cross-paradigm modelling, maximize parallelism, and improve power efficiency
- To demonstrate the utility of building a brain-like cross-paradigm system, we designed an unmanned bicycle experiment by deploying multiple specialized networks in parallel within one Tianjic chip
- Equipped with versatile algorithms and models, the bicycle was able to perform real-time object detection, tracking, voice-command recognition, riding over a speed bump, obstacle avoidance, balance control and decision making
- To integrate these networks and achieve high-level decision-making, we developed an SNN-based neural state machine (NSM)
- The NSM receives the inputs from other networks (CNN, SNN), and outputs enabling signals (CNN, CANN) and action signals (for example, forced turn, obstacle avoidance) to downstream FCores for bicycle motor control. 
- Before the road test, the CNN, CANN, SNN and MLP networks were pretrained and programmed onto the Tianjic chip

## Conclusion 

In summary, we have developed the Tianjic chip, which supports both computer-science-based, machine-learning algorithms and neuroscience-based, biologically inspired models simultaneously. 
Various neural networks and hybrid coding schemes can be freely integrated, allowing for seamless communication among multiple networks, including SNNs and ANNs. 
Our research has examined a novel neuromorphic architecture that offers flexibility by integrating cross-paradigm models and algorithms onto a single platform; we hope that our findings will accelerate the development of AGI, with many possible real-world applications.

## My Notes

Havent justified artificial general intelligence in the context of generic ML framework. 
What they meant was a hybrid and reconfigurable framework for implementing any ML algorithm on a single platform.

[1]: https://www.nature.com/articles/s41586-019-1424-8
