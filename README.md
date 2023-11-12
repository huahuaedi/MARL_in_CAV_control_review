<!-- omit in toc -->
# Multi-Agent Reinforcement Learning for Connected and Automated Vehicles Control: Recent Advancements and Future Prospects


A curated list of awesome **Multi-Agent Reinforcement Learning in Connected and Automated Vehicles Control** papers 🔥🔥🔥. 



**<font color='red'>Work still in progress</font>**  🚀, **we appreciate any suggestions and contributions** ❤️.

---

<!-- What is multi-agent reinforcement learning?
Why multi-agent reinforcement learning?
-->

<!-- TODO
## Our scope:
We aim to stay up-to-date with the most innovative developments in the field and gain valuable insights into the future of multi-agent reinforcement learning technology.👀 organize a systematic and comprehensive overview of multi-agent reinforcement learning.

1. Stay up-to-date with the most innovative developments in this field.
2. Gain valuable insights into the future of multi-agent reinforcement learning technology.
3. 
-->


<!-- omit in toc -->
## How to contribute?

If you have any suggestions or find any missed papers, feel free to reach out or submit a [pull request](https://github.com/huahuaedi/MARL_in_CAV_control/pulls):

1. Use following markdown format.

```markdown
*Author 1, Author 2, and Author 3.* **Paper Title.**  <ins>Conference/Journal/Preprint</ins> Year. [[pdf](link)]; [[other resources](link)].
```
<!-- >1. **Paper Title.** *Author 1, Author 2, and Author 3.* Conference/Journal/Preprint Year. [[pdf](link)]. -->

2. If one preprint paper has multiple versions, please use **the earliest submitted year**.
   
3. Display the papers in a **year descending order** (the latest, the first).


<!-- omit in toc -->
## Citation

Find this repository helpful? 😊  

Please consider citing our paper. 👇👇👇

*(**Note that the current version of our survey is only a draft, and we are still working on it.**)* 🚀

<!-- ```
@article{li2023label,
  title={Label-Efficient Learning in Agriculture: A Comprehensive Review},
  author={Li, Jiajia and Chen, Dong and Qi, Xinda and Li, Zhaojian and Huang, Yanbo and Morris, Daniel and Tan, Xiaobo},
  journal={arXiv preprint arXiv:2305.14691},
  year={2023}
}
```-->

<!-- TODO: add survey citation and link -->

<!-- omit in toc -->
## 🔍 Table of Contents 

- [1. 💁🏽‍♀️ Introduction](#1-️-introduction)
-    [1.1. Development of CAV Control](#11-development-of-cav-control)
-    [1.2. Contributions of this review](#12-contributions-of-this-review)
- [2. 🗂️ Backgrounds](#2-️-backgrounds)
  - [2.1 Preliminaries of Reinforcement Learning](#21-preliminaries-of-reinforcement-learning)
      - [2.1.1 Deep Q-Learning](#211-deep-q-learning)
      - [2.1.2 Policy Gradient](#212-policy-gradient)
      - [2.1.3 Actor-critic Network](#213-actor-critic-network)
  - [2.2 Multi-Agent Reinforcement Learning](#22-multi-agent-reinforcement-learning)
  - [2.3 Training and Execution Strategies in MARL](#23-training-and-execution-strategies-in-marl)
      - [2.3.1 Centralized training with decentralized execution](#231-centralized-training-with-decentralized-execution)
      - [2.3.2 Decentralized training with decentralized execution](#232-decentralized-training-with-decentralized-execution)
  - [2.4 MARL Algorithm Variants](#24-marl-algorithm-variants)
      - [2.4.1 Value function decomposition](#241-value-function-decomposition)
      - [2.4.2 Learning to Communicate](#242-learning-to-communicate)
- [3. 🤖 Towards applications in connected and autonomous vehicles](#3--towards-applications-in-connected-and-autonomous-vehicles)
  - [3.1 One-dimensional Cooperation](#31-one-dimensional-cooperation)
  - [3.2 Two-dimensional Cooperation](#32-two-dimensional-cooperation)
  - [3.3 Three-dimensional Cooperation](#33-three-dimensional-cooperation)
      - [3.3.1 Traffic signal control](#321-traffic-signal-control)
      - [3.3.2 On-ramps merging](#322-on-ramps-merging)
      - [3.3.3 Unsignalized intersections](#322-unsignalized-intersections)
  - [3.4 Simulation platforms](#33-simulation-platforms)
- [4. 📚 Corpora](#4--corpora)
- [5. 📖 Extended Reading](#5--extended-reading)
  - [5.1 Instruction Induction](#51-instruction-induction)
  
---


## 1. 💁🏽‍♀️ Introduction
### 1.1 Development of CAV Control]

![image](https://github.com/huahuaedi/MARL_in_CAV_control_review/blob/main/cav_framework.png)

### 1.2 Contributions of this review

Why multi-agent reinforcement learning on the extent of control dimensions for connected and automated vehicles(CAVs)?


- 👉 **Joint Policy Learning.**  Unlike traditional control methods or single-agent reinforcement learning, **MARL allows for the simultaneous learning of multiple decision-makers (agents).** This joint policy learning enables CAVs to develop cooperative strategies that are necessary for tasks like synchronized lane changing, platooning, or intersection management.
- 👉 **Partial Observability and Information Sharing.**  CAVs might not be able to observe the entire traffic situation due to line-of-sight limitations, sensor range, or communication constraints.  **MARL algorithms can be designed to allow agents to make decisions based on partial information and to learn how to infer the missing information through interaction, which may include strategies for selective information sharing.**
- 👉 **Scalable Learning and Decentralized Execution.** Provides a framework for scalable learning by allowing each agent to learn from its local observations while still considering the global outcome. **This can also lead to decentralized execution, where each CAV operates based on its policy without the need for a central controller, thus making the system more robust to single points of failure.** ![](https://img.shields.io/badge/-platooning%20control-yellow)  ![](https://img.shields.io/badge/-lane--changing%20control-red) ![](https://img.shields.io/badge/-traffic%20signal%20control-orange) ![](https://img.shields.io/badge/-on--ramps%20merging-brightgreen) ![](https://img.shields.io/badge/-unsignalized%20intersections-blue)



 
1. Wang, Wenshuo, et al. **"Social interactions for autonomous driving: A review and perspectives."** Foundations and Trends® in Robotics 10.3-4 (2022): 198-376.  [[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Social+interactions+for+autonomous+driving%3A+A+review+and+perspectives&btnG=) [[Paper]](https://www.nowpublishers.com/article/Details/ROB-078) 

2. Fei-Yue Wang. **"Artificial intelligence and intelligent transportation: Driving into the 3rd axial age with ITS"** International Conference on Algorithmic Learning Theory. Springer, Berlin, Heidelberg, 2006.  [[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Artificial+intelligence+and+intelligent+transportation%3A+Driving+into+the+3rd+axial+age+with+ITS&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8082803) 

3. Wei, Liu, et al. **"A Systematic Survey of Control Techniques and Applications in Connected and Automated Vehicles."** IEEE Access 9 (2021): 82146-82168.  [[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=A+Systematic+Survey+of+Control+Techniques+and+Applications+in+Connected+and+Automated+Vehicles&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10225497) 


## 2. 🎓 Backgrounds

In our paper, we divide the textual instructions into three categories.

### 2.1 Multi-agent System for CAV Control


### 2.2 Preliminaries of Reinforcement Learning (RL)

#### 2.2.1 Deep Q-Learning

#### 2.2.2 Policy Gradient

#### 2.2.3 Actor-critic Network


### 2.3 Multi-Agent Reinforcement Learning (MARL)



### 2.4 Training and Execution Strategies in MARL

#### 2.4.1 Centralized training with decentralized execution (CTDE)



#### 2.4.2 Decentralized training with decentralized execution (DTDE)



### 2.5 MARL Algorithm Variants

#### 2.5.1 Value function decomposition



#### 2.5.2 Learning to Communicate



#### 2.5.3 Hierarchical structure
1. Arthur, David, and Sergei Vassilvitskii. **"K-means++ the advantages of careful seeding."** Proceedings of the eighteenth annual ACM-SIAM symposium on Discrete algorithms. 2007. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=K-means%2B%2B+the+advantages+of+careful+seeding&btnG=) [[Paper]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=K-means%2B%2B+the+advantages+of+careful+seeding&btnG=) 

#### 2.5.4 Causal inference


## 3. 🤖 Towards applications in connected and autonomous vehicles


### 3.1 One-dimensional Cooperation

Instructions are used in various human-computer interaction (HCI) tasks, such as virtual assistants, chatbots, etc. 

1. Coletta, Luiz FS, et al. **"Novelty detection in UAV images to identify emerging threats in eucalyptus crops."** Computers and Electronics in Agriculture 196 (2022): 106901. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Novelty+detection+in+UAV+images+to+identify+emerging+threats+in+eucalyptus+crops&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169922002186?casa_token=ZFhy1QK7aakAAAAA:wI-NrE3CAa8ph4hZ_iuU-qB0hXz6c6Kpn4f5P301ZI7qxFC4R6mxiOOogDMET4qBwo8zhARxUnE)  

 


### 3.2 Two-dimensional Cooperation

1. Marszalek, Michael L., et al. **"Self-supervised learning--A way to minimize time and effort for precision agriculture?."** arXiv preprint arXiv:2204.02100 (2022). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Self-supervised+learning--A+way+to+minimize+time+and+effort+for+precision+agriculture%3F&btnG=) [[Paper]](https://arxiv.org/abs/2204.02100) 



### 3.3 Three-dimensional Cooperation

#### 3.3.1 Traffic signal control
1. Mofan Zhou, et al. **"Development of an efficient driving strategy for connected and automated vehicles at signalized intersections: A reinforcement learning approach."** Computers and Electronics in Agriculture 205 (2023): 107624. [[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Development+of+an+efficient+driving+strategy+for+connected+and+automated+vehicles+at+signalized+intersections%3A+A+reinforcement+learning+approach&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8848852)  


#### 3.3.2 On-ramps merging

1. Kong, Qingchen, et al. **"A recurrent network based on active learning for the assessment of fish feeding status."** Computers and Electronics in Agriculture 198 (2022): 106979. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+recurrent+network+based+on+active+learning+for+the+assessment+of+fish+feeding+status&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169922002964?casa_token=3sEdz3v21LgAAAAA:Xt0sn8l-FcWHyTSPuTPg-zR1nIkH59hhu0yl2uju8z2kDi2yjGVYfIo-egNbffOruatbiO4C6Qw)  


#### 3.3.3 Unsignalized intersections

1. Lin, Xufeng, et al. **"Self-Supervised Leaf Segmentation under Complex Lighting Conditions."** Pattern Recognition 135 (2023): 109021. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Self-Supervised+Leaf+Segmentation+under+Complex+Lighting+Conditions&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0031320322005015?casa_token=hbczlttXx3QAAAAA:Sj_D4jBQEBfVQpM2H1V3KTVqvFyzz1rvErGPqMFFIdVWSqiJMJMYONoWnRHGONStKrc4p-Vt0oM)  [[Code]](https://github.com/lxfhfut/Self-Supervised-Leaf-Segmentation) 




#### 3.3.4 Simulation Platforms
1. Liu, Yisen, et al. **"Joint optimization of autoencoder and self-supervised classifier: anomaly detection of strawberries using hyperspectral imaging."** Computers and Electronics in Agriculture 198 (2022): 107007. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Joint+optimization+of+autoencoder+and+Self-Supervised+Classifier%3A+Anomaly+detection+of+strawberries+using+hyperspectral+imaging&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169922003246?casa_token=mbiSlzaiRvEAAAAA:6rfTcrs7MG1etkv2cGSz75ZfjBAUc0OdCa5l32TvDYmXNrqJ2iRcbNjC4Ee-F-rq4L0bLx3gz_4)  


<!-- TODO: tweets & slides? -->

---

<!-- omit in toc -->
