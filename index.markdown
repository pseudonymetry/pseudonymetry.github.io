---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

title: Closing the Loop for Accountable Interference-free Spectrum Sharing with Passive Radio Receivers
layout: default
---

# Closing the Loop for Accountable Interference-free Spectrum Sharing with Passive Radio Receivers

## Project Description

Spectrum in the US is incredibly valuable to science, education, commerce, transportation, and contemporary life. Wireless bandwidth needs are rapidly growing, but allocation of spectrum to wireless users should not come at the expense of scientific observation in astronomy and earth science which are already under-allocated and subject to interference when operating opportunistically outside the narrow protected bands. This project is developing new secure and accountable sharing protocols that not only enable more efficient sharing of the spectrum between terrestrial commercial wireless systems and passive receivers, but also empowers passive systems to force a particular interfering transmitter to switch band. Improved coexistence allows more reliable operation of radio astronomy receivers. This project is creating open source software and data, and working with the ITU-R to ensure that results impact the research community and future spectrum sharing policy. Developments are impacting undergraduate and graduate education through course material and research experiences, and the project is engaged in K12 outreach.

This project is developing RF watermarks that embed random pseudonyms into transmitted wireless communication signals so that passive receivers can demodulate the pseudonym of any interferer. The proposed system then allows passive receivers to indirectly inform the interfering device to change band. To prevent any other device from inferring private information, the proposed system leverages differential privacy to quantitatively limit privacy leakage. Further, the project is adapting software attestation to develop proof of correct execution of spectrum decision on user equipment, and complementing the watermark-based detection system with spectrum policy enforcement. Protocols under study are being implemented and tested on PAWR testbeds as an open source project. Extensive experimentation, including at the Owens Valley Radio Observatory, is validating the technical contributions, and quantifying its performance and robustness to attacks.

## Team

<p>
**[Neal Patwari](https://engineering.wustl.edu/faculty/Neal-Patwari.html)** (<a href="mailto:neal.patwari@gmail.com">neal.patwari@gmail.com</a>) at Washington University in St. Louis   
<br>**[Ning Zhang](https://engineering.wustl.edu/faculty/Ning-Zhang.html)** (<a href="mailto:zhang.ning@wustl.edu">zhang.ning@wustl.edu</a>) at Washington University in St. Louis
<br>**[Greg Hellbourg](https://directory.caltech.edu/personnel/ghellbou)** (<a href="mailto:greg.hellbourg@gmail.com">greg.hellbourg@gmail.com</a>) at California Institute of Technology 
</p>

<center><img src="logos/washu-logo.png" alt="WashU_logo" height="50"/><img src="logos/caltech-new-logo.png" alt="CalTech_logo" height="50"/></center>



## Background

**Spectrum Sharing**
<!-- <iframe width="600" height="360" src="https://www.youtube.com/watch?v=de4O8ZrldpU" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/de4O8ZrldpU" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


<!-- **Differential Privacy**
<iframe width="560" height="315" src="https://www.youtube.com/embed/gI0wk1CXlsQ" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


**Software Attestation**
<iframe width="560" height="315" src="https://www.youtube.com/embed/22ttDmu3VMY" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> -->

## Research Publication
<p>
  ARI: Attestation of Real-time Mission Execution Integrity [<a href="https://www.usenix.org/system/files/usenixsecurity23-wang-jinwen.pdf">PDF</a>]
    <br> J. Wang, Y. Wang, A. Li, Y. Xiao, R. Zhang, W. Lou, Y. Hou, N. Zhang
    <br> USENIX Security Symposium, 2023
</p>

## Open Source Repositories
<p>
  ARI: Attestation of Real-time Mission Execution Integrity [<a href="https://github.com/WUSTL-CSPL/ARI">Github Repo</a>]
</p>


## Acknowledgement

This project is supported by NSF under award #2229427.


<!-- 
## Team
HeatDeCam was developed by the following team of academica researchers:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**[Zhiyuan Yu](https://zh1yu4nyu.github.io/)** at Washington University in St. Louis  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**[Zhuohang Li](http://web.eecs.utk.edu/~zli96/)** at University of Tennessee, Knoxville  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**[Yuanhaur Chang](https://changoliver.github.io/)** at Washington University in St. Louis  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**[Skylar Fong](https://www.linkedin.com/in/skylarfong/)** at Washington University in St. Louis  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**[Jian Liu](https://web.eecs.utk.edu/~jliu/)** at University of Tennessee, Knoxville  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**[Ning Zhang](https://engineering.wustl.edu/faculty/Ning-Zhang.html)** at Washington University in St. Louis  

<p style='text-align: center'> Contact us at <a href="mailto:yu.zhiyuan@wustl.edu">yu.zhiyuan@wustl.edu</a></p>

<center><img src="logos/WUSTL.png" alt="WashU_logo" width="200"/><img src="logos/UTK.jpg" alt="UTK_logo" width="170"/></center>

## Features

**Motivation of This Work**

This work is motivated by the gap of existing detection methods and our obervations on the heat dissipation patterns of spy cameras.

There have been both commercial products and research prototypes that leverage radiofrequency (RF) signals and optical reflections to detect spy cameras. While achieving impressive detection performance, they could be limited in detecting non-wirelessly connected cameras and usability. To fill the gap, we leverage thermal imagery as the detection vector. An example of heat dissipation patterns in shown in the figures below. 

<center><img src="figs/Angle1.png" alt="Angle1" width="200"/><img src="figs/Angle2.png" alt="Angle2" width="200"/></center>

We observe that the spy camera disguised as a charger plug (at the top in black) exhibits additional uneven heat distribution, as compared to the regular charger plug (at the bottom in white). This is because spy cameras have to add unique hardware components (e.g., SD cards, image sensors) without changing the original form factor. It will unavoidable affect internal layout that was originally optimized for heat dissipation. 

**Key Approach**

However, it is almost impossible that we require users to manually distinguish heat patterns with their raw eyes. We develop a data-driven approach with designed neural network model to recognize and locate the spy cameras.

We collect the first thermal image dataset of spy cameras. It consists of over 22,056 images collected from six rooms across three scenarios, Airbnb, hotel, and office. A total of eleven heterogeneous spy cameras with varying properties in apperances, functionalities, brands, costs.

<center><img src="figs/Spycams.jpg" alt="Spycams" width="230"/>&nbsp;&nbsp;<img src="figs/Rooms.png" alt="Rooms" width="260"/></center>

The overall workflow of our detection algorithm is depicted in the figure.

<center><img src="figs/Workflow.png" alt="Workflow" width="830"/></center>

The key design elements include:

- Thermal-visual registration to align spatial features
- Adaptive soft mask to mitigate environmental influences while preserving context
- Neural-network-based feature extraction and recognition 
- CAM-based visualization of hidden locations of spy cameras

The structural design of the neural network incorporates ResNet-based feature extration and attention module that enables effective learning of heat pattern features.

<center><img src="figs/NeuralNetwork.png" alt="NeuralNetwork" width="600"/></center>

**Experiments in the Real World**

We developed an Android app as a prototype of our approach. Besides evaluation on our collected dataset, we also invited people to use our prototype to find hidden spy cameras deployed in a simulated room. Our method is shown to be superior to commercial products in both detection rate and false positive. To test the robustness in high-temperature environments, we also conduct experiments in a room with temperature over 104°F.

<center><img src="figs/Detectors.jpg" alt="Detectors" width="230"/>&nbsp;&nbsp;<img src="figs/InPersonRoom.jpg" alt="Room" width="230"/>&nbsp;&nbsp;<img src="figs/AdvEnv.png" alt="AdvEnv" width="172"/></center>

For more details of our work, please see our [paper](https://dl.acm.org/doi/10.1145/3548606.3560669). Also please contact us if you have any questions! -->
