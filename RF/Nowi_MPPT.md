# [Energy-Efficient Low-Power Circuit Techniques for Wireless Energy and Data Transfer in IoT Sensor Nodes][1]

A new [MS thesis](http://elca.tudelft.nl/Education/thesisdetails.php?ti=265) topic was hosted in their university website.</br>
Follow this project's progress by visitng [Prof. Wouter A. Serdijn](https://scholar.google.com/citations?user=ZLxC4EMAAAAJ&hl=en) profile.

### Key Points
- We focus on the RF Energy Harvester (RFEH), the data receiver and the transmitter, all of which have a large impact on the device cost, lifetime and functionality.
- Codesign of the antenna and the electronics is explored to boost the power conversion efficiency of the RF-DC converter.
- As a proof of principle, a charge pump rectifier is designed, and its measurement results are presented. 
- To boost the rectifier output voltage, a DC-DC converter that employs maximum power point tracking has been designed.
- A prototype circuit is also presented that can accommodate an input power level range of 1 µW to 1 mW and offers peak efficiencies of 76.3% and 82% at 1 µW and 1 mW, respectively.
- The co-design principle is also used at the receiver side where the antenna-electronics interface is optimized.
- It is shown how this technique allows improving the noise figure of the Low Noise Amplifier (LNA) without sacrificing power consumption.

### Conclusion
The circuit techniques presented in this paper allow to have both energy and bidirectional data transfer to a sensor node in a low-power and energy-efficient manner. 
Five different scenarios of antenna configurations in which a WSN can operate and how those circuit techniques can be applied in those scenarios have been described. 
The three fundamental blocks considered are: RF to DC converter, data receiver and data transmitter. 
With repect to the RF-DC conversion, a voltage boosting network combined with a 5-stage on-chip rectifier and its measurement results were presented. 
A DC-DC converter was presented as an alternative to a multistage onchip rectifier. 
The implemented buck-boost DC-DC converter employs an MPPT technique that estimates the input power, and adjusts the equivalent input resistance of the DC-DC converter in order to maximize the power extracted from the rectifier, allowing for efficient harvesting across a larger range of available input power. 
Regarding both the RF-DC conversion and the data receiver, we showed that co-design of the antenna and electronics leads to better performance for the overall system. 
For the data receiver, the co-design technique leads to better performance in terms of NF and power efficiency, and for the RF-DC converter it leads to better power conversion efficiency by boosting the rectifier input voltage. 
In order to achieve low-power data transmission, the task that usually consumes the most power in a WSN, a novel low-power sub-GHz UWB transmitter was presented along with its measurement results. 
Throughout the paper a quantified comparison with some relevant prior art, has been carried out, proving that the power gap present in the state of the art WSNs can be drastically reduced, or even disappear.

### My Notes
After watching a video on Linedin highlighting the uniqueness of Nowi's MPPT. 
They claim that it outperfoms any other MPPT chips in market with smaller footprint without the need of any external components.

In the paper 5 different configurations of antenna and usage in terms of EH, RF Tx and RF Rx and some tradeoffs using existing literature work is discussed. 



[1]: https://arxiv.org/abs/1704.08910
