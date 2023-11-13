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
-    [1.1. Multi-agent System for CAV Control](#11-multi-agent-system-for-cav-control)
-    [1.2. Contributions of this review](#12-contributions-of-this-review)
- [2. 🗂️ Backgrounds](#2-️-backgrounds)
  - [2.1 Preliminaries of Reinforcement Learning](#21-preliminaries-of-reinforcement-learning)
      - [2.1.1 Deep Q-Learning](#211-deep-q-learning)
      - [2.1.2 Policy Gradient](#212-policy-gradient)
      - [2.1.3 Actor-critic Network](#213-actor-critic-network)
  - [2.2 Multi-Agent Reinforcement Learning](#22-multi-agent-reinforcement-learning)
  - [2.3 Training and Execution Strategies in MARL](#23-training-and-execution-strategies-in-marl)
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
### 1.1 Multi-agent System for CAV Control

![image](https://github.com/huahuaedi/MARL_in_CAV_control_review/blob/main/cav_framework.png)

### 1.2 Contributions of this review

Why multi-agent reinforcement learning on the extent of control dimensions for connected and automated vehicles(CAVs)?


- 👉 **Joint Policy Learning.**  Unlike traditional control methods or single-agent reinforcement learning, **MARL allows for the simultaneous learning of multiple decision-makers (agents).** This joint policy learning enables CAVs to develop cooperative strategies that are necessary for tasks like synchronized lane changing, platooning, or intersection management.
- 👉 **Partial Observability and Information Sharing.**  CAVs might not be able to observe the entire traffic situation due to line-of-sight limitations, sensor range, or communication constraints.  **MARL algorithms can be designed to allow agents to make decisions based on partial information and to learn how to infer the missing information through interaction, which may include strategies for selective information sharing.**
- 👉 **Scalable Learning and Decentralized Execution.** Provides a framework for scalable learning by allowing each agent to learn from its local observations while still considering the global outcome. **This can also lead to decentralized execution, where each CAV operates based on its policy without the need for a central controller, thus making the system more robust to single points of failure.** ![](https://img.shields.io/badge/-platooning%20control-yellow)  ![](https://img.shields.io/badge/-lane--changing%20control-red) ![](https://img.shields.io/badge/-traffic%20signal%20control-orange) ![](https://img.shields.io/badge/-on--ramps%20merging-brightgreen) ![](https://img.shields.io/badge/-unsignalized%20intersections-blue)

1. Wang, Wenshuo, et al. **"Social interactions for autonomous driving: A review and perspectives."** Foundations and Trends® in Robotics 10.3-4 (2022): 198-376. 
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Social+interactions+for+autonomous+driving%3A+A+review+and+perspectives&btnG=) [[Paper]](https://www.nowpublishers.com/article/Details/ROB-078) 

2. Wang, Fei-Yue. **"Artificial intelligence and intelligent transportation: Driving into the 3rd axial age with ITS"** IEEE Intelligent transportation systems magazine 9.4 (2017): 6-9.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Artificial+intelligence+and+intelligent+transportation%3A+Driving+into+the+3rd+axial+age+with+ITS&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8082803) 

3. Liu, Wei, et al. **"A systematic survey of control techniques and applications in connected and automated vehicles."** IEEE Internet of Things Journal (2023).
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=A+Systematic+Survey+of+Control+Techniques+and+Applications+in+Connected+and+Automated+Vehicles&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10225497) 

4. Schmidt, Lukas M., et al. **"An introduction to multi-agent reinforcement learning and review of its application to autonomous mobility."** 2022 IEEE 25th International Conference on Intelligent Transportation Systems (ITSC). IEEE, 2022.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=An+introduction+to+multi-agent+reinforcement+learning+and+review+of+its+application+to+autonomous+mobility&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9922205) 

5. Dinneweth, Joris, et al. **"Multi-agent reinforcement learning for autonomous vehicles: A survey."** Autonomous Intelligent Systems 2.1 (2022): 27.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Multi-agent+reinforcement+learning+for+autonomous+vehicles%3A+A+survey&btnG=) [[Paper]](https://link.springer.com/article/10.1007/s43684-022-00045-z) 

## 2. 🎓 Backgrounds
### 2.1 Preliminaries of Reinforcement Learning (RL)

1. Kaelbling, Leslie Pack, Michael L. Littman, and Andrew W. Moore. **"Reinforcement learning: A survey."** Journal of artificial intelligence research 4 (1996): 237-285.
[[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Reinforcement+learning%3A+A+survey&btnG=) [[Paper]](https://www.jair.org/index.php/jair/article/view/10166/24110) 

2. Arulkumaran, Kai, et al. **"Deep reinforcement learning: A brief survey."** IEEE Signal Processing Magazine 34.6 (2017): 26-38.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Deep+reinforcement+learning%3A+A+brief+survey&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8103164) 

3. Wang, Hao-nan, et al. **"Deep reinforcement learning: a survey."** Frontiers of Information Technology & Electronic Engineering 21.12 (2020): 1726-1744.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Deep+reinforcement+learning%3A+a+survey&btnG=) [[Paper]](https://link.springer.com/article/10.1631/FITEE.1900533) 

4. **Reinforcement Learning: An Introduction.** 
 [[Code]](https://github.com/dennybritz/reinforcement-learning) 

5. Li, Yuxi. **"Deep reinforcement learning: An overview."** arXiv preprint arXiv:1701.07274 (2017).
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=DEEP+REINFORCEMENT+LEARNING&btnG=) [[Paper]](https://arxiv.org/pdf/1810.06339v1.pdf) 

6. Varuna Jayasiri, Nipun Wijerathne. **labml.ai Annotated Paper Implementations.**
[[Code]](https://nn.labml.ai/)

#### 2.1.1 Deep Q-Learning

1. Mnih, Volodymyr, et al. "Playing atari with deep reinforcement learning." arXiv preprint arXiv:1312.5602 (2013).
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Playing+Atari+with+Deep+Reinforcement+Learning&btnG=) [[Paper]](https://arxiv.org/pdf/1312.5602v1.pdf)  [[Code]](https://github.com/ray-project/ray/tree/master/rllib/algorithms/dqn) 

2.
[[Google Scholar]]() [[Paper]]()  [[Code]]()

3.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

4.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

5.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

6.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 


#### 2.1.2 Policy Gradient

1. Schulman, John, et al. **"Proximal policy optimization algorithms."** arXiv preprint arXiv:1707.06347 (2017).
[[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Proximal+policy+optimization+algorithms&btnG=) [[Paper]](https://arxiv.org/pdf/1707.06347.pdf)  [[Code]]() 

2.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

3.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

4.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

5.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

6.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

#### 2.1.3 Actor-critic Network
1.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

2.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

3.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

4.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

5.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

### 2.2 Multi-Agent Reinforcement Learning (MARL)
1. Nguyen, Thanh Thi, Ngoc Duy Nguyen, and Saeid Nahavandi. **"Deep reinforcement learning for multiagent systems: A review of challenges, solutions, and applications."** IEEE transactions on cybernetics 50.9 (2020): 3826-3839.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Deep+reinforcement+learning+for+multiagent+systems%3A+A+review+of+challenges%2C+solutions%2C+and+application&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9043893) 

2. Gronauer, Sven, and Klaus Diepold. **"Multi-agent deep reinforcement learning: a survey."** Artificial Intelligence Review (2022): 1-49.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Multi-agent+deep+reinforcement+learning%3A+a+survey&btnG=) [[Paper]](https://link.springer.com/article/10.1007/s10462-021-09996-w) 

3. Zhang, Kaiqing, Zhuoran Yang, and Tamer Başar. **"Multi-agent reinforcement learning: A selective overview of theories and algorithms."** Handbook of reinforcement learning and control (2021): 321-384.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Multi-agent+reinforcement+learning%3A+A+selective+overview+of+theories+and+algorithms&btnG=) [[Paper]](https://link.springer.com/chapter/10.1007/978-3-030-60990-0_12) 

4. Tan, Ming. **"Multi-agent reinforcement learning: Independent vs. cooperative agents."** Proceedings of the tenth international conference on machine learning. 1993.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Multi-agent+reinforcement+learning%3A+Independent+vs.+cooperative+agents.&btnG=) [[Paper]](https://books.google.co.uk/books?hl=zh-CN&lr=&id=TrqjBQAAQBAJ&oi=fnd&pg=PA330&dq=Multi-agent+reinforcement+learning:+Independent+vs.+cooperative+agents.&ots=v3_fYV6XSn&sig=ePsM7WCM6EwxuPiclMg1xyx8H8c&redir_esc=y#v=onepage&q=Multi-agent%20reinforcement%20learning%3A%20Independent%20vs.%20cooperative%20agents.&f=false) 

5. Nguyen, Thanh Thi, Ngoc Duy Nguyen, and Saeid Nahavandi. **"Deep reinforcement learning for multiagent systems: A review of challenges, solutions, and applications."** IEEE transactions on cybernetics 50.9 (2020): 3826-3839.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Deep+reinforcement+learning+for+multiagent+systems%3A+A+review+of+challenges%2C+solutions%2C+and+applications&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9043893) 

6. Chen, Hao. **"Multi-Agent Reinforcement Learning Papers with Code."**
[[Code]](https://github.com/TimeBreaker/MARL-papers-with-code) 


### 2.3 Training and Execution Strategies in MARL

#### 2.3.1 Centralized training with decentralized execution (CTDE)
1.
[[Google Scholar]]() [[Paper]]() 

2.
[[Google Scholar]]() [[Paper]]() 

3.
[[Google Scholar]]() [[Paper]]() 

4.
[[Google Scholar]]() [[Paper]]() 

5.
[[Google Scholar]]() [[Paper]]() 

1.
[[Google Scholar]]() [[Paper]]() 

2.
[[Google Scholar]]() [[Paper]]() 

3.
[[Google Scholar]]() [[Paper]]() 

4.
[[Google Scholar]]() [[Paper]]() 

5.
[[Google Scholar]]() [[Paper]]() 

6.
[[Google Scholar]]() [[Paper]]() 

### 2.4 MARL Algorithm Variants

#### 2.4.1 Value function decomposition

1. Son, Kyunghwan, et al. **"Qtran: Learning to factorize with transformation for cooperative multi-agent reinforcement learning."** International conference on machine learning. PMLR, 2019.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=QTRAN%3A+Learning+to+Factorize+with+Transformation+for+Cooperative+Multi-Agent+Reinforcement+learning&btnG=) [[Paper]](https://arxiv.org/pdf/1905.05408.pdf) [[Code]](https://github.com/oxwhirl/pymarl)

2. Rashid, Tabish, et al. **"Monotonic value function factorisation for deep multi-agent reinforcement learning."** The Journal of Machine Learning Research 21.1 (2020): 7234-7284.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Monotonic+value+function+factorisation+for+deep+multi-agent+reinforcement+learning&btnG=) [[Paper]](https://proceedings.mlr.press/v80/rashid18a/rashid18a.pdf)  [[Code]](https://github.com/oxwhirl/pymarl)

3. Sunehag, Peter, et al. **"Value-decomposition networks for cooperative multi-agent learning."** arXiv preprint arXiv:1706.05296 (2017).
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Value-Decomposition+Networks+For+Cooperative+Multi-Agent+Learning&btnG=) [[Paper]](https://arxiv.org/pdf/1706.05296.pdf)  [[Code]](https://github.com/oxwhirl/pymarl) 

4. 
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

5.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

6.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

#### 2.4.2 Learning to Communicate

1. Sukhbaatar, Sainbayar, and Rob Fergus. **"Learning multiagent communication with backpropagation."** Advances in neural information processing systems 29 (2016).
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Learning+multiagent+communication+with+backpropagation&btnG=) [[Paper]](https://arxiv.org/pdf/1605.07736.pdf)  [[Code]](https://github.com/facebookarchive/CommNet)

2. Foerster, Jakob, et al. **"Learning to communicate with deep multi-agent reinforcement learning."** Advances in neural information processing systems 29 (2016).
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Learning+to+communicate+with+deep+multi-agent+reinforcement+learning&btnG=) [[Paper]](https://proceedings.neurips.cc/paper_files/paper/2016/file/c7635bfd99248a2cdef8249ef7bfbef4-Paper.pdf) 

3. Peng, Peng, et al. **"Multiagent bidirectionally-coordinated nets: Emergence of human-level coordination in learning to play starcraft combat games."** arXiv preprint arXiv:1703.10069 (2017).
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Multiagent+Bidirectionally-Coordinated+Nets+Emergence+of+Human-level+Coordination+in+Learning+to+Play+StarCraft+Combat+Games&btnG=) [[Paper]](https://arxiv.org/pdf/1703.10069.pdf)  [[Code]](https://github.com/Coac/CommNet-BiCnet) 

4. Singh, Amanpreet, Tushar Jain, and Sainbayar Sukhbaatar. **"Learning when to communicate at scale in multiagent cooperative and competitive tasks."** arXiv preprint arXiv:1812.09755 (2018).
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=LEARNING+WHEN+TO+COMMUNICATE+AT+SCALE+IN+MULTIAGENT+COOPERATIVE+AND+COMPETITIVE+TASKS&btnG=) [[Paper]](https://arxiv.org/pdf/1812.09755.pdf)  [[Code]](https://github.com/IC3Net/IC3Net) 

5. Foerster, Jakob, et al. **"Learning to communicate with deep multi-agent reinforcement learning."** Advances in neural information processing systems 29 (2016).
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Learning+to+Communicate+with+Deep+Multi-Agent+Reinforcement+Learning&btnG=) [[Paper]](https://arxiv.org/pdf/1605.06676.pdf)  [[Code]](https://github.com/iassael/learning-to-communicate) 

6.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 


#### 2.4.3 Hierarchical structure
1. Pateria, Shubham, et al. **"Hierarchical reinforcement learning: A comprehensive survey."** ACM Computing Surveys (CSUR) 54.5 (2021): 1-35.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Hierarchical+reinforcement+learning%3A+A+comprehensive+survey&btnG=) [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3453160) 

2.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

3.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

4.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

5.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

#### 2.4.4 Causal inference

1. Grimbly, St John, Jonathan Shock, and Arnu Pretorius. **"Causal multi-agent reinforcement learning: Review and open problems."** arXiv preprint arXiv:2111.06721 (2021).
[[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Causal+multi-agent+reinforcement+learning%3A+Review+and+open+problems&btnG=) [[Paper]](https://arxiv.org/pdf/2111.06721.pdf)  

2. Jaques, Natasha, et al. **"Intrinsic social motivation via causal influence in multi-agent RL."** (2018).
[[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Intrinsic+social+motivation+via+causal+influence+in+multi-agent+RL&btnG=) [[Paper]](https://openreview.net/forum?id=B1lG42C9Km)  [[Code]](https://www.catalyzex.com/paper/arxiv:1810.08647/code) 

3. Wang, Han, Yang Yu, and Yuan Jiang. **"Fully Decentralized Multiagent Communication via Causal Inference."** IEEE Transactions on Neural Networks and Learning Systems (2022).
[[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Fully+Decentralized+Multiagent+Communication+via+Causal+Inference&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9761961) 

4. 
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

5.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 

6.
[[Google Scholar]]() [[Paper]]()  [[Code]]() 



## 3. 🤖 Towards applications in connected and autonomous vehicles

In this section, we will comprehensively explore the recent strides made in the utilization of MARL within CAV applications. Our examination will be structured according to various dimensions of cooperation, each correlated with a specific number of control components. 

**One-dimensional cooperation** corresponds to scenarios involving control along a single control direction, such as either longitudinal control or lateral control. ![](https://img.shields.io/badge/-platooning%20control-yellow) 

**Two-dimensional cooperation** extends the scope to include both longitudinal and lateral control components, reflecting the increased complexity in the coordination and decision-making of CAVs. ![](https://img.shields.io/badge/-lane--changing%20control-red)

**Three-dimensional cooperation** further augments the challenges and opportunities by incorporating additional constraints, such as time limits, which encompass aspects like traffic light control and on-ramp merging. ![](https://img.shields.io/badge/-traffic%20signal%20control-orange) ![](https://img.shields.io/badge/-on--ramps%20merging-brightgreen) ![](https://img.shields.io/badge/-unsignalized%20intersections-blue)

### 3.1 One-dimensional Cooperation

1. Parvini, Mohammad, et al. **"AoI-aware resource allocation for platoon-based C-V2X networks via multi-agent multi-task reinforcement learning."** IEEE Transactions on Vehicular Technology (2023).
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=AoI-aware+resource+allocation+for+platoon-based+C-V2X+networks+via+multi-agent+multi-task+reinforcement+learning&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10077432)  

2. He, Lv. **"Multi-vehicle Platoon Overtaking Using NoisyNet Multi-Agent Deep Q-Learning Network."** arXiv preprint arXiv:2303.02583 (2023).
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Multi-vehicle+Platoon+Overtaking+Using+NoisyNet+Multi-Agent+Deep+Q-Learning+Network&btnG=) [[Paper]](https://arxiv.org/pdf/2303.02583.pdf) 

3. Xu, Yuanyuan, et al. **"Deep Reinforcement Learning for Multi-Objective Resource Allocation in Multi-Platoon Cooperative Vehicular Networks."** IEEE Transactions on Wireless Communications (2023).
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Deep+Reinforcement+Learning+for+Multi-Objective+Resource+Allocation+in+Multi-Platoon+Cooperative+Vehicular+Networks&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10040608) 

4. Beaver, Logan E. **"Constraint-driven optimal control of multiagent systems: A highway platooning case study."** IEEE Control Systems Letters 6 (2021): 1754-1759.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Constraint-driven+optimal+control+of+multiagent+systems%3A+A+highway+platooning+case+study&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9642048) 

5. Li, Yongfu, et al. **"Consensus-based cooperative control for multi-platoon under the connected vehicles environment."** IEEE Transactions on Intelligent Transportation Systems 20.6 (2018): 2220-2229.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Consensus-based+cooperative+control+for+multi-platoon+under+the+connected+vehicles+environment&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8458142) 

6. Guo, Xiang-Gui, et al. **Multi-agent systems: platoon control and non-fragile quantized consensus.** CRC Press, 2019.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Multi-agent+systems%3A+platoon+control+and+non-fragile+quantized+consensus&btnG=) [[Paper]](https://books.google.co.uk/books?hl=zh-CN&lr=&id=iU-fDwAAQBAJ&oi=fnd&pg=PP1&dq=Multi-agent+systems:+platoon+control+and+non-fragile+quantized+consensus&ots=bzvsfmRvjQ&sig=L3Hbh5yh3cHKfuATXyrT7mzW_nM&redir_esc=y#v=onepage&q=Multi-agent%20systems%3A%20platoon%20control%20and%20non-fragile%20quantized%20consensus&f=false) 

7. Li, Yongfu, et al. **"Platoon control of connected multi-vehicle systems under V2X communications: Design and experiments."** IEEE Transactions on Intelligent Transportation Systems 21.5 (2019): 1891-1902.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Platoon+control+of+connected+multi-vehicle+systems+under+V2X+communications%3A+Design+and+experiments&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8686052) 


### 3.2 Two-dimensional Cooperation

1. Zhou, Wei, et al. **"Multi-agent reinforcement learning for cooperative lane changing of connected and autonomous vehicles in mixed traffic."** Autonomous Intelligent Systems 2.1 (2022): 5.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Multi-agent+reinforcement+learning+for+cooperative+lane+changing+of+connected+and+autonomous+vehicles+in+mixed+traffic&btnG=) [[Paper]](https://link.springer.com/article/10.1007/s43684-022-00023-5) 

2. Chen, Sikai, et al. **"Graph neural network and reinforcement learning for multi‐agent cooperative control of connected autonomous vehicles."** Computer‐Aided Civil and Infrastructure Engineering 36.7 (2021): 838-857.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Graph+neural+network+and+reinforcement+learning+for+multi-agent+cooperative+control+of+connected+autonomous+vehicles&btnG=) [[Paper]](https://onlinelibrary.wiley.com/doi/epdf/10.1111/mice.12702) 

3. Candela, Eduardo, et al. **"Transferring multi-agent reinforcement learning policies for autonomous driving using sim-to-real."** 2022 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, 2022.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Transferring+multi-agent+reinforcement+learning+policies+for+autonomous+driving+using+sim-to-real&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9981319) 

4. Le, Nguyen-Tuan-Thanh. **"Multi-agent reinforcement learning for traffic congestion on one-way multi-lane highways."** Journal of Information and Telecommunication (2023): 1-15.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Multi-agent+reinforcement+learning+for+traffic+congestion+on+one-way+multi-lane+highways&btnG=) [[Paper]](https://www.tandfonline.com/doi/epdf/10.1080/24751839.2023.2182174?needAccess=true) 

5. Chen, Siyuan, et al. **"Multi-Agent Reinforcement Learning-Based Decision Making for Twin-Vehicles Cooperative Driving in Stochastic Dynamic Highway Environments."** IEEE Transactions on Vehicular Technology (2023).
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Multi-Agent+Reinforcement+Learning-Based+Decision+Making+for+Twin-Vehicles+Cooperative+Driving+in+Stochastic+Dynamic+Highway+Environments&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10123696) 

6. Zong, Fang, et al. **"Dynamic lane changing trajectory planning for CAV: A multi-agent model with path preplanning."** Transportmetrica B: transport dynamics 10.1 (2022): 266-292.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Dynamic+lane+changing+trajectory+planning+for+CAV%3A+A+multi-agent+model+with+path+preplanning&btnG=) [[Paper]](https://www.tandfonline.com/doi/epdf/10.1080/21680566.2021.1989079?needAccess=true) 

7. Zhang, Jiawei, et al. **"Multi-agent DRL-based lane change with right-of-way collaboration awareness."** IEEE Transactions on Intelligent Transportation Systems 24.1 (2022): 854-869.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Multi-agent+DRL-based+lane+change+with+right-of-way+collaboration+awareness&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9932003) 


### 3.3 Three-dimensional Cooperation

#### 3.3.1 Traffic signal control
1. Antonio, Guillen-Perez, and Cano Maria-Dolores. **"Multi-agent deep reinforcement learning to manage connected autonomous vehicles at tomorrow's intersections."** IEEE Transactions on Vehicular Technology 71.7 (2022): 7033-7043.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Multi-Agent+Deep+Reinforcement+Learning+to+Manage+Connected+Autonomous+Vehicles+at+Tomorrow%27s+Intersections&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9762548)  

2. Liu, Junjia, et al. **"Learning scalable multi-agent coordination by spatial differentiation for traffic signal control."** Engineering Applications of Artificial Intelligence 100 (2021): 104165.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Learning+scalable+multi-agent+coordination+by+spatial+differentiation+for+traffic+signal+control&btnG=) [[Paper]](https://pdf.sciencedirectassets.com/271095/1-s2.0-S0952197621X00024/1-s2.0-S0952197621000129/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjEAEaCXVzLWVhc3QtMSJGMEQCIAnDQt2PUtRjdejaqxutROY%2BTSmCNbxbCgxfbDB9GGnBAiB0C6v5puId9gWnULkA6DuB845e6Zt%2Bvv7rag83K1MzySqyBQhJEAUaDDA1OTAwMzU0Njg2NSIMudM3oNTRcDdiPKkjKo8FX6oM%2FlO6mqT57gKHPd57Pv0JEvT1XC32LEy9sfAAQJcIoTQ%2FZfk9xf3feNeoOfB2Uaw20Vo%2BA5rm3bcRzkr9FbyqglBuyxlKgpxIDG8U3BY1QcfY9Csw3Ih70CLfdjhg%2F%2FNa0CXEWzjN2iB9%2FRqr%2BkJRrjlKMqwmhIz%2FvTBf7wHbBOb8%2Fg6p6vrl1CBJzA8doNZg7zeWXgP%2BVxWdySeLkzu%2BsbsmCAPqY4NdSvIK8z8oGimRqRtgIvFYLb2B8vJ%2BzoTfkaNZUkvT3UH1Z1zSXaHk2hhzgLBOvqdf%2Bs2Iu628Hviyr7GhnEI%2BEXyySXWXJF3UgFi1PUD3dWy5xMqjjBDD9LvuAUxVwDYyxaI7tf4J0ds6OoCj8BhWuuNRELLR8RRWdQ3cmtM11SvnG9cHucIXyrqEwl1WID%2BNQjXP6aHrlUwpY5VmzexjFL2x4UaucyJTv4OK%2FMYKaH%2BlPU5yQexZpMw%2FebYgzjRt6u63O5%2Bytj7o8A3cUt4Y0o2GJI%2B2v5aEzk3p%2FPXUDpgO6dmsjmhqyTIHLdvoMNvoBTMku1QYSFZL0jd91St5GboZ3FYhIKkLERu%2BmPM9sOdUpYbHzVxV9v9h5Vx1kbUQk%2BtTrS1DNADqUTMz6kYtfboDTw%2BHq0xIVW4PxhHJbudcy4%2FhqfySliuZG%2FHNILypBs7QvXT9wTmLm8%2FREcpukc8MGdPStQfaDLTjUcB7hVmK8x55tEJK1uVXgvvluGbd%2FnrYPOhMKUlYnuTt%2F7EaZmS6K3vD8Gdz4MW9iI3gW%2B5UPJYgkuJaMbZvTtM3B4YqdRwlp5pMCHdY%2FzTdMij3ynnZsboSWK4qn%2FMoDyPtHqb519MvNtDDdSrpSncLZXWkc33hVjCemMmqBjqyAWOLpJtl%2Bm6jFTUO3opASaYrLUmFjD5oKjdwYjyGrHDYwyU%2B5T1cSLoBREa2qntmqVb16PElJ79Jtpfx%2B%2BVTgkLYGCMYOvzq%2F7tLghJhA84Rh4ljjCL37LoVTfbdxnV75lx1iizJZNtKBf7r%2F3w35%2F5jRQFZKO%2FXYvGbKhxlY%2BW7DJ0ir7BhIJm0PvuFzALTv0NhPooejH%2BhoUt1wMapbaBaMwjs8%2BaK6veaMzJMDTUpiWk%3D&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20231113T175220Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTY5TETT7M4%2F20231113%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=00322a2e698ed6aaa279ea229d6db1e8070bf81a9609a25180a8c8dc7d32a6af&hash=70912cada3c65db1f7d84a3e886b248bccf990a256822e2ddfabab8e6ca02838&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0952197621000129&tid=spdf-4cd930d7-4df7-4559-8561-7d71fc042fc6&sid=f4f7fa4920e573475449386-60b9f94d1dcdgxrqb&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=1d075c515a5806025c&rr=8258de2c1cdd63f1&cc=gb) 

3. Liu, Dongjiang, and Leixiao Li. **"A traffic light control method based on multi-agent deep reinforcement learning algorithm."** Scientific Reports 13.1 (2023): 9396.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=A+traffic+light+control+method+based+on+multi-agent+deep+reinforcement+learning+algorithm&btnG=) [[Paper]](https://www.nature.com/articles/s41598-023-36606-2) 

4. Wang, Yanan, et al. **"STMARL: A spatio-temporal multi-agent reinforcement learning approach for cooperative traffic light control."** IEEE Transactions on Mobile Computing 21.6 (2020): 2228-2242.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=STMARL%3A+A+spatio-temporal+multi-agent+reinforcement+learning+approach+for+cooperative+traffic+light+control&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9240060) 

5. Ma, Jinming, and Feng Wu. **"Feudal multi-agent deep reinforcement learning for traffic signal control."** Proceedings of the 19th International Conference on Autonomous Agents and Multiagent Systems (AAMAS). 2020.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Feudal+multi-agent+deep+reinforcement+learning+for+traffic+signal+control&btnG=) [[Paper]](http://staff.ustc.edu.cn/~wufeng02/doc/htm/MWaamas20.html?lang=zh) 

6. Wang, Tong, Jiahua Cao, and Azhar Hussain. **"Adaptive Traffic Signal Control for large-scale scenario with Cooperative Group-based Multi-agent reinforcement learning."** Transportation research part C: emerging technologies 125 (2021): 103046.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Adaptive+Traffic+Signal+Control+for+large-scale+scenario+with+Cooperative+Group-based+Multi-agent+reinforcement+learning&btnG=) [[Paper]](https://pdf.sciencedirectassets.com/271729/1-s2.0-S0968090X21X00022/1-s2.0-S0968090X21000760/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjEAEaCXVzLWVhc3QtMSJGMEQCIAnDQt2PUtRjdejaqxutROY%2BTSmCNbxbCgxfbDB9GGnBAiB0C6v5puId9gWnULkA6DuB845e6Zt%2Bvv7rag83K1MzySqyBQhJEAUaDDA1OTAwMzU0Njg2NSIMudM3oNTRcDdiPKkjKo8FX6oM%2FlO6mqT57gKHPd57Pv0JEvT1XC32LEy9sfAAQJcIoTQ%2FZfk9xf3feNeoOfB2Uaw20Vo%2BA5rm3bcRzkr9FbyqglBuyxlKgpxIDG8U3BY1QcfY9Csw3Ih70CLfdjhg%2F%2FNa0CXEWzjN2iB9%2FRqr%2BkJRrjlKMqwmhIz%2FvTBf7wHbBOb8%2Fg6p6vrl1CBJzA8doNZg7zeWXgP%2BVxWdySeLkzu%2BsbsmCAPqY4NdSvIK8z8oGimRqRtgIvFYLb2B8vJ%2BzoTfkaNZUkvT3UH1Z1zSXaHk2hhzgLBOvqdf%2Bs2Iu628Hviyr7GhnEI%2BEXyySXWXJF3UgFi1PUD3dWy5xMqjjBDD9LvuAUxVwDYyxaI7tf4J0ds6OoCj8BhWuuNRELLR8RRWdQ3cmtM11SvnG9cHucIXyrqEwl1WID%2BNQjXP6aHrlUwpY5VmzexjFL2x4UaucyJTv4OK%2FMYKaH%2BlPU5yQexZpMw%2FebYgzjRt6u63O5%2Bytj7o8A3cUt4Y0o2GJI%2B2v5aEzk3p%2FPXUDpgO6dmsjmhqyTIHLdvoMNvoBTMku1QYSFZL0jd91St5GboZ3FYhIKkLERu%2BmPM9sOdUpYbHzVxV9v9h5Vx1kbUQk%2BtTrS1DNADqUTMz6kYtfboDTw%2BHq0xIVW4PxhHJbudcy4%2FhqfySliuZG%2FHNILypBs7QvXT9wTmLm8%2FREcpukc8MGdPStQfaDLTjUcB7hVmK8x55tEJK1uVXgvvluGbd%2FnrYPOhMKUlYnuTt%2F7EaZmS6K3vD8Gdz4MW9iI3gW%2B5UPJYgkuJaMbZvTtM3B4YqdRwlp5pMCHdY%2FzTdMij3ynnZsboSWK4qn%2FMoDyPtHqb519MvNtDDdSrpSncLZXWkc33hVjCemMmqBjqyAWOLpJtl%2Bm6jFTUO3opASaYrLUmFjD5oKjdwYjyGrHDYwyU%2B5T1cSLoBREa2qntmqVb16PElJ79Jtpfx%2B%2BVTgkLYGCMYOvzq%2F7tLghJhA84Rh4ljjCL37LoVTfbdxnV75lx1iizJZNtKBf7r%2F3w35%2F5jRQFZKO%2FXYvGbKhxlY%2BW7DJ0ir7BhIJm0PvuFzALTv0NhPooejH%2BhoUt1wMapbaBaMwjs8%2BaK6veaMzJMDTUpiWk%3D&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20231113T175655Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTY5TETT7M4%2F20231113%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=7d7588fb3328db76a0ebe8b5d609a8fab3e62594edf9c4e22d4d7a28d6ad62df&hash=af4106491097c4c545997a017930a81b4edc8419bde92febe78f5191a331e196&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0968090X21000760&tid=spdf-bcb93093-7f33-4c6d-ac87-0a404f5a08a9&sid=f4f7fa4920e573475449386-60b9f94d1dcdgxrqb&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=1d075c515a5807530b&rr=8258e4e30fae63f1&cc=gb) 

7. Yang, Shantian, et al. **"IHG-MA: Inductive heterogeneous graph multi-agent reinforcement learning for multi-intersection traffic signal control."** Neural networks 139 (2021): 265-277.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=IHG-MA%3A+Inductive+heterogeneous+graph+multi-agent+reinforcement+learning+for+multi-intersection+traffic+signal+control&btnG=) [[Paper]](https://pdf.sciencedirectassets.com/271125/1-s2.0-S0893608021X00044/1-s2.0-S0893608021000952/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjEAEaCXVzLWVhc3QtMSJIMEYCIQD0uwT2eM%2F1ccJ04yAo5l7onE6ATvesuiEIYzYGz6PDSQIhAO2fVa0NG6NP9N2sA23JnMA%2FW0PcD77DkQV5YLCBZT%2BHKrMFCEkQBRoMMDU5MDAzNTQ2ODY1IgxgNRrluSJ11CeuWuoqkAUJJAdY3qBdfDxUbCiDVIrJUMyuG2JPuTRBh4355%2BptYfTD7iac6fWZjOpO4CBDoVzbq%2FKgMckjVuqjEDpfiYxo8qvoFvVdk0aFfmqa3emhx5fVPnHjiJ9eXo75xhCkfDWV7KHF7WPgrT0NKThXv8s%2FVqx6mpuaamAqQA8YviMlSxRMwsGaqQNTBsCZhHwV5dshlzDSITZo30bcI9nBcbT1nouDWSqvRvWrBdmZ8cSNcdBRUmcz5FgTrcP5QDy3I7R9m%2BL0%2BsupL9B97GyH4ihN3%2FXi4A7tmRMP%2BdSKtu8vtKNruPEfhIlE4H%2BfQ7MEtXF%2Fi%2FvsGATc8wWIeyOCMJnac6DDDZNRdYwWCIjRP7UPjfJGU8CEac0sGODyFpko7J1zr6bq%2Bv%2B%2FEI80keyr44G47maYMiUQg9UsHE3jpOeS8%2B7VAgrxNPCSs%2B5PK%2FVKCOJoFtmPf7zARjQGDU0O9iIWmNFj0b27UQmUWu6BQGXq%2FLggya%2FnArEuLtlfD3orzxeFaGArfzkS%2Bw08WQzTsBj9wrC8Bn7VC5hAKQ4UmS9piY%2Bi5PE2w37dDU%2FSNnIMjZOoR%2B8G3YEA1rKzQZthroJ%2BswYFJQNe8y%2FFdFpZuUFidao55VQO3En7h43FkTt4JBdpH%2F4LEzFFf77gZO5am6qDeNbzRAseoWwUYo%2FHVmV%2BH7KlHm7A8zTEXL6FTBcBYbnALHlg9HZ0BZaGserLCIGLUc3hJJPBfWNF0OUnYzbGgTT9gcUlSwDYkky8CICf3hV1%2BYD4xPKfcr%2BBkgmxls0zENLcdjxnC4oFoJT6G4g6CZfamt6b4wCbUWvUnWVYJUoTkWIo2swVDgwPDn1%2FIuDO%2F2oSapPW0CLfZ4%2BpPvfAuDDdmMmqBjqwAfwfWQa9zFEEHhYGMHszJ0YCkhHwmjjuK6IfVjr65q%2B4mzT3VtClmjgfZ1qAMK%2FpV8O2nlA478MBx4BVDl6qQPLcbUb9hV%2FoSfW1vukpm6DMs8emhDmSshJpfkSDZ1F5jP1afj7%2B9NT15T%2BV4NzFHIipjodbY4SZCftMK9T4g2qEFaGSOhu%2B3yRkLrytS%2BKyrCincy4uqKBQedB1eNUkbXCkMqvKtOgkvZ676A95iom5&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20231113T175834Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTYZ3QRNYUL%2F20231113%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=90542804196bbe17add793af2845b654f7d096e3a6c6b45988c88f1ab474941a&hash=cd367b1737af4b76ceac68c2671ff9f7afebcd6419540fe9730f2ecd6055af07&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0893608021000952&tid=spdf-4b2c7fb6-0ee2-4643-bfe7-6b58050e828c&sid=f4f7fa4920e573475449386-60b9f94d1dcdgxrqb&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=1d075c515a5807505b&rr=8258e7539a1963f1&cc=gb) 

#### 3.3.2 On-ramps merging

1. Chen, Dong, et al. **"Deep multi-agent reinforcement learning for highway on-ramp merging in mixed traffic."** IEEE Transactions on Intelligent Transportation Systems (2023).
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Deep+multi-agent+reinforcement+learning+for+highway+on-ramp+merging+in+mixed+traffic&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10159552)  

2. Chandra, Rohan, and Dinesh Manocha. **"Gameplan: Game-theoretic multi-agent planning with human drivers at intersections, roundabouts, and merging."** IEEE Robotics and Automation Letters 7.2 (2022): 2676-2683.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Gameplan%3A+Game-theoretic+multi-agent+planning+with+human+drivers+at+intersections%2C+roundabouts%2C+and+merging%7D%2C+++author%3D%7BChandra%2C+Rohan+and+Manocha%2C+Dinesh&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9689991) 

3. Hu, Yeping, et al. **"Interaction-aware decision making with adaptive strategies under merging scenarios."** 2019 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, 2019.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Interaction-aware+decision+making+with+adaptive+strategies+under+merging+scenarios&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8968478) 

4. Schester, Larry, and Luis E. Ortiz. **"Longitudinal position control for highway on-ramp merging: A multi-agent approach to automated driving."** 2019 IEEE Intelligent Transportation Systems Conference (ITSC). IEEE, 2019.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Longitudinal+position+control+for+highway+on-ramp+merging%3A+A+multi-agent+approach+to+automated+driving&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8916951) 

5. Li, Lin, et al. **"Nash double Q-based multi-agent deep reinforcement learning for interactive merging strategy in mixed traffic."** Expert Systems with Applications 237 (2024): 121458.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Nash+double+Q-based+multi-agent+deep+reinforcement+learning+for+interactive+merging+strategy+in+mixed+traffic&btnG=) [[Paper]](https://pdf.sciencedirectassets.com/271506/1-s2.0-S0957417423X00244/1-s2.0-S0957417423019607/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjEAQaCXVzLWVhc3QtMSJGMEQCIB6ulxC2qpE24MKXilOZE2B252ACc9dwpKEIaMCoBIrzAiBDZXvQvK8cIqUltCxqBZZFBv9X2yc1PbdsZoP71xmQbyqzBQhMEAUaDDA1OTAwMzU0Njg2NSIMTM4c16SiJUdoBsEjKpAF%2B7fOHlLaLudlO3ryBfDisCebD3w3G7dLHQScln%2FBRZFpDoU5gd%2F%2BIEaAgx0D5uBW0GQJ3hKMKEM49pc5nUn2EV9SYk2BOHxj8164JYy2iDfaku3eOzPBeu4ag02pbK9kPUIKMn5JdkV7uDuOXcUssQZml8cHFGwmyGgoep%2Fo8Anw0yP9X%2BpF3EI5IKUE4MslRhSw8zJuTdqhHHeiG%2B6ee%2BBKb0YRxlhIA%2FXBLR%2BmBbwKimCr%2BLb1ivcRAiavAWZg8N36SuGEKd%2FLhXOIVpyUPLYgJHT%2FEJmVDk6ykfgaS%2BFVQhjIZj%2BYFeHlatPz7DghdFd4XkZxLL6MqrlK6HHgspZbqgsj7oYyl1re8RV%2B18mfuQNGS0MELQ6hu%2BpvxzH%2Fq0nYbwnjdXV2cEe6LhS0QopQmkXa1YfYeAMu6Ko1ETsP1VffR5hl2UxgUXqNkYqXxGNL3ljQdMq8zal9HWxYa8Oa6fqKgt4mX%2BbpoTErcRRrvyv1%2FCNvZGXqArtcaorixQ1x1sEXNvmGm1drtjqk6VdNmX0ImJljV0Svz9PypRQ8nvgUGtUQyr2RRYWC%2Fda2BzjptOwG1XIRNxIigBLNg9B7gPJlzLPv%2FW650Py12aol7CoZHyJx4%2BiU4WgydQLZt1KYYh9Ms5iHNICmCImjOGQ1PNXnt1wxP%2FTKwNMsrS7UL8GrHVz0HS5GdHgf5Q4fiDrQLBPDZp1xu3ckxaTYTfUIy7CCUS3Cul9kHypiAbkKzkmztq05dxGyp85qFiRIpxsPZepm7x%2F7QQg8GvaCbAPmue936XeTTOBAIdGOMBlHIEy2klDLcFRK5PO8e5PxbS7BAMFyNWlpDcMRyypmKr49BBMrwZy6Z0MU7c%2FdLa4wpurJqgY6sgH%2FqyloAE%2FKlNXhd14%2BWohtRgwaXcBuE%2BR23BtQ8bHyRdJRHQaJTb2rvahZH6BB7PfPBiaIuvisuY6ljS9p%2Bzyof4HGujMBQrbZTbgrW1%2BSjqpJiub%2Buwr5BhgR2TkirpnL%2BVJg%2Fzsbkkv2URNvZnwB28%2BhtpVaEiPJh23tyxc68YqHRo4MDF9rQAHiKpYk4RXu9Zecg%2FW3DS37yUfcXo18ftmlcZHVlBwmgmhAeCB6Adz1&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20231113T203510Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTY672L3DMA%2F20231113%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=009918c85b65257040ce28c9e941a41297795c81ad8e4507b88f2541f21cab70&hash=b8e7aa83ace7808cd1ce1796503ee31a5b517453e4cfedc50b05fc8c2bb20b1d&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0957417423019607&tid=spdf-28d022f6-358e-4a3d-a41d-090695f2af47&sid=f4f7fa4920e573475449386-60b9f94d1dcdgxrqb&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=1d075c515a5901040c&rr=8259ccb4ca61240c&cc=gb) 

6. Zhang, Xinfeng, et al. **"High-Speed Ramp Merging Behavior Decision for Autonomous Vehicles Based on Multi-Agent Reinforcement Learning."** IEEE Internet of Things Journal (2023).
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=High-Speed+Ramp+Merging+Behavior+Decision+for+Autonomous+Vehicles+Based+on+Multi-Agent+Reinforcement+Learning&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10215357) 

7. Zine, el abidine Kherroubi, Samir Aknine, and Rebiha Bacha. **"Novel decision-making strategy for connected and autonomous vehicles in highway on-ramp merging."** IEEE Transactions on Intelligent Transportation Systems 23.8 (2021): 12490-12502.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Novel+decision-making+strategy+for+connected+and+autonomous+vehicles+in+highway+on-ramp+merging&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9557770) 

#### 3.3.3 Unsignalized intersections

1. Spatharis, Christos, and Konstantinos Blekas. **"Multiagent reinforcement learning for autonomous driving in traffic zones with unsignalized intersections."** Journal of Intelligent Transportation Systems (2022): 1-17.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Multiagent+reinforcement+learning+for+autonomous+driving+in+traffic+zones+with+unsignalized+intersections&btnG=) [[Paper]](https://www.tandfonline.com/doi/epdf/10.1080/15472450.2022.2109416?needAccess=true) 

2. Bautista-Montesano, Rolando, et al. **"Autonomous navigation at unsignalized intersections: A coupled reinforcement learning and model predictive control approach."** Transportation research part C: emerging technologies 139 (2022): 103662.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Autonomous+navigation+at+unsignalized+intersections%3A+A+coupled+reinforcement+learning+and+model+predictive+control+approach&btnG=) [[Paper]](https://pdf.sciencedirectassets.com/271729/1-s2.0-S0968090X22X00053/1-s2.0-S0968090X2200105X/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjEAEaCXVzLWVhc3QtMSJGMEQCIGV6LOCDLwIgL63NjZmS9IZuY40OCndPXyWJMFyuh0axAiALrmCkv%2Bf2QbU7MdPbD7pj5Q8Bf701kELio4KFT2J4aSqyBQhKEAUaDDA1OTAwMzU0Njg2NSIMJjsvOtYABjlk78leKo8Fzap2BhK3FrpXbziDlQwr%2FMxMuYinJbyGmz4iRpYH5G0POcjN6IKQVbW3TPC0BrMMcHTSMzAzlhsAT%2BqCFhXG6TMng9fsLYvBSwwcAggVEvPhFivcvaN9m7uMFH87zNMlJFCgoWWwXGdehMuWxp7gbDg5FXf5DNuNaIT79Ae%2F3r64PJ7THe4uR9EaW0kYup9YLEneUAEVUuptIKWW18WuFigORSPLZ3oyr89%2BdQt3RS1EUAsifLFq0YIB6Z%2F1iUlPfwsZ5TNz0v7yUt6DsjrkBoS6XFNOtf38fPpGZGeZVnMCg7KWMeWT5YAxphGcSzElws5dvLCopQhtNvUlHzN08i%2FvuJJ8dCqXKXTsQcu2GuToU6akkXfRrn1GkmGjjK0q%2FvkNHZW5zYnNKwyOwlUFAAOhaVCuA4%2FB9ML4k6L6G7%2BCCqjvZ3krxRCZqVgxCoXBV9%2BhRIllwOmGqFqt%2Fu6hsCox7Z%2FqHVa2tRMkkyI82AY2ScUNV6RnfQDbBS5XE4%2BHuOaAu%2Byq71E2pnpDNB6CQB5wfROm0cU9tJkAKaYtYlVvq4LfXyFmOf8dQTNxb7UW3xwBM1pSpWHHZyX4By0KluyJasLfpdPGQDU%2Fzjy2qZsVpZGJC03bCNfFvtCug7JIk1XBKsZ2%2BV5kiFM5gp2CGv2%2B8ot4rFXYwu%2BCkd4lswh579D%2BsXf5sHIxfK5Gi5izF4NNGcPo2YJKhz0NE6v8%2B6P8UeHLR6egfPZkzVTgpqR1u9HLyIazlujaZEW5Q1BqiANYO7jf6iPJrsXfOBcv%2BhDEUtB0FBv%2F%2FKrR4i1BtzNsy8Ycgi9sfjw0s51dQ%2FKCKhWhmwoC4zFKK6%2F%2F36Do0uI3dqk9OLGrc0ezSniN6jCAqMmqBjqyAf6s5DU9BNYyce7Lo0i10o1wcDJXSxoF%2BGsgJUCxLVBxZUgrClaAABsPsw1GR%2FHiC9dBuw97tDoV2w1Ub5g%2B3o%2B%2Bx3%2B040B86x9bh08ftbNYLuPL6523%2BdT9Y60nTfdhg7%2B9M0PT0uFD5n9qr1bk3io3t4W49WlVcKgD6lu6BNFSqze0x6KkJiTRFaWoENLsMLbR7S6DrO9St7u83rwNgIl%2Bft3B2Zf%2Bhdk13AfDm9MP5Q4%3D&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20231113T180909Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTYTBRIILEE%2F20231113%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=e62e148c803f4dfcf97dcff0c94f62e9ae80b42828bc51e7c258eaf4c6b49cfe&hash=af8cb9ee50a38f0c6d7af0ad406463a820a35844c30b6d190210f53545f000e2&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0968090X2200105X&tid=spdf-b41f2773-d659-4177-96b3-d59b0810a895&sid=f4f7fa4920e573475449386-60b9f94d1dcdgxrqb&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=1d075c515a5804510a&rr=8258f6d2fe5f63d4&cc=gb) 

3. Shu, Hong, et al. **"Driving tasks transfer using deep reinforcement learning for decision-making of autonomous vehicles in unsignalized intersection."** IEEE Transactions on Vehicular Technology 71.1 (2021): 41-52.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Driving+tasks+transfer+using+deep+reinforcement+learning+for+decision-making+of+autonomous+vehicles+in+unsignalized+intersection&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9583858) 

4. Peng, Bile, et al. **"Connected autonomous vehicles for improving mixed traffic efficiency in unsignalized intersections with deep reinforcement learning."** Communications in Transportation Research 1 (2021): 100017.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Connected+autonomous+vehicles+for+improving+mixed+traffic+efficiency+in+unsignalized+intersections+with+deep+reinforcement+learning&btnG=) [[Paper]](https://pdf.sciencedirectassets.com/780746/1-s2.0-S2772424721X00029/1-s2.0-S2772424721000172/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjEAIaCXVzLWVhc3QtMSJGMEQCIEkejgCOF5DupJ1CNDF6g%2B1giKiW5WhoFttYi90hfiIZAiB1dRmp4VeOzFcspFpM0AjfE6blebNECC40V4aQfyI1%2FSqyBQhLEAUaDDA1OTAwMzU0Njg2NSIMu1E53Le4mrhT5FJhKo8FXvt3gdEbKi6XjF3GACSnlZOBJhTwZV%2BRv2RfJUqNoDOBu8ljGJC3wJoYJekph8f8yCl3n0uFwWBGI07Imt6NbjNiOtHg2V7jd8T6KiacNjDKXdDaC%2F%2Ba%2B85TPBPEURAbz2m6V3Er0ph2WagXrGg9xbVARrQ61IljMmKh1hyBCC4%2BlvT1S1yFWpscSSkJ1sa2S0HqjiBzoeg9I1LDmyZ6SSSzKacDnIo%2FguZ8g4O6jEgiTAOO8hNVHSdg%2F9H21BzjIvUo6mvEs1CIwNeD0f0RqNZEjQ1rfemrFpb3oD4flarKdHPCf1qcGsb9bDGt30TdBnbt2qAT%2B4I1slFxWjGfr7HlkjwGDYv7EQaZWfKqedfH%2B8GowrBRSc%2FSPAvCKODVS864jqvTxEbpoDyYNNrf5AKl8qP8OvhFJuSU8ai%2BZEBkvNnuOQkqgBL3ceVlROvE%2B49%2BzpwUT0YPiJblJsSpdF%2BbyvBozvIRk1f6c95jVJ9npF%2BYUPzH60z9o%2BZ554tJoM54%2FkxR2VNRY8xZGLVGsHudf3Zlj1pfy6GNLS0MYO8gzPMdF4Pg0o0oaZu3WG4gFLQlMUnxPmw8dN4VY%2B4LmUTow3ZlVosRlXFFYJFz1%2FTEd9%2FXTJgf%2F6l5q11ubuuTeSSe2kNkO88KBYoQYxwGChpFjQFlCB4CQtEPl%2BwKud64JCHWNloBdMcSg2CSwlYvLmk3nMOTumnnbyMdF0UR%2B2dfhKS%2BCqwlF50Pc9ZZkMFyRqD%2B4uVl05YGFErdLhVYNRTy5cHWpAKGAQYTXVauReQJ%2FqHe8VNXWpMroGsnk5mA49YlX9wyLTfd9JG8IFecmulOi80dArR1RHjQNQb1SzFgjrMHCWKdIlCUe2f0ozCTucmqBjqyAYoTCTnYFy1NroKn1lcAVqc7gBCy1sP7iyquPnVVrF3vx4SQm4w5CLoLwxlKiRmUEFbIqOSq77FtQrDSSPuvG9X2xyxMf9delxEv58Q5hhc0lrPOUMaKWLNVSXCbA71Y3CrXu6aot%2BejkZ4ClPbmMFKbIZL6Dv96tDy2fCO3kMxP0ycNX6p48QNWIbHSiAaRp2PSP5o%2Bij7Z42KXeCsPotWhgy4dWMhfhcPN4wzxgJE8zIg%3D&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20231113T181109Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTY3HPNJEU4%2F20231113%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=3a35f684bd2f267b1bfbf8465c3fbc4e53ec617655fe0115f1b1c037873baf6c&hash=b8a2eb283442b32e6ac363b448e17d6bc6531b977e611382c0776398e102dac6&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S2772424721000172&tid=spdf-15d1e163-df62-4f01-bf0c-30f19a62aa14&sid=f4f7fa4920e573475449386-60b9f94d1dcdgxrqb&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=1d075c515a58045e0c&rr=8258f9bc4c1148bf&cc=gb) 

5. Guo, Zihan, et al. **"Coordination for connected and automated vehicles at non-signalized intersections: A value decomposition-based multiagent deep reinforcement learning approach."** IEEE Transactions on Vehicular Technology 72.3 (2022): 3025-3034.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Coordination+for+connected+and+automated+vehicles+at+non-signalized+intersections%3A+A+value+decomposition-based+multiagent+deep+reinforcement+learning+approach&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9939107) 

6. Geng, Maosi, et al. **"Multimodal Vehicular Trajectory Prediction With Inverse Reinforcement Learning and Risk Aversion at Urban Unsignalized Intersections."** IEEE Transactions on Intelligent Transportation Systems (2023).
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Multimodal+Vehicular+Trajectory+Prediction+With+Inverse+Reinforcement+Learning+and+Risk+Aversion+at+Urban+Unsignalized+Intersections&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10164651) 

7. Xu, Yunting, et al. **"Leveraging multiagent learning for automated vehicles scheduling at nonsignalized intersections."** IEEE Internet of Things Journal 8.14 (2021): 11427-11439.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Leveraging+multiagent+learning+for+automated+vehicles+scheduling+at+nonsignalized+intersections&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9336022) 

   
#### 3.3.4 Simulation Platforms
1. Dosovitskiy, Alexey, et al. **"CARLA: An open urban driving simulator."** Conference on robot learning. PMLR, 2017.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=CARLA%3A+An+open+urban+driving+simulator&btnG=) [[Paper]](https://proceedings.mlr.press/v78/dosovitskiy17a/dosovitskiy17a.pdf)   [[Code]](https://github.com/carla-simulator/carla)

2. Zhang, Huichu, et al. **"Cityflow: A multi-agent reinforcement learning environment for large scale city traffic scenario."** The world wide web conference. 2019.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0,5&q=Cityflow:+A+multi-agent+reinforcement+lear+Cityflow:+A+multi-agent+reinforcement+lear) [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3308558.3314139)  [[Code]](https://github.com/cityflow-project/CityFlow/) 

3. Zhou, Ming, et al. **"Smarts: Scalable multi-agent reinforcement learning training school for autonomous driving."** arXiv preprint arXiv:2010.09776 (2020).
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Smarts%3A+Scalable+multi-agent+reinforcement+learning+training+school+for+autonomous+driving&btnG=) [[Paper]](https://arxiv.org/pdf/2010.09776.pdf)  [[Code]](https://github.com/huawei-noah/SMARTS) 

4. Li, Quanyi, et al. **"Metadrive: Composing diverse driving scenarios for generalizable reinforcement learning."** IEEE transactions on pattern analysis and machine intelligence 45.3 (2022): 3461-3475.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Metadrive%3A+Composing+diverse+driving+scenarios+for+generalizable+reinforcement+learning&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9829243)  [[Code]](https://github.com/metadriverse/metadrive) 

5. Lopez, Pablo Alvarez, et al. **"Microscopic traffic simulation using sumo."** 2018 21st international conference on intelligent transportation systems (ITSC). IEEE, 2018.
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Microscopic+traffic+simulation+using+sumo&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8569938)  [[Code]](https://github.com/eclipse-sumo/sumo/tree/main) 

6. Leurent, Edouard. **"An environment for autonomous driving decision-making."** (2018).
[[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=An+Environment+for+Autonomous+Driving+Decision-Making&btnG=) [[Code]](https://github.com/Farama-Foundation/HighwayEnv) 


<!-- TODO: tweets & slides? -->

---

<!-- omit in toc -->
