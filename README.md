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
  - [2.1 Multi-agent system for CAV Control](#21-multi-agent-system-for-cav-control)
  - [2.2 Preliminaries of Reinforcement Learning](#22-preliminaries-of-reinforcement-learning)
      - [2.2.1 Deep Q-Learning](#221-deep-q-learning)
      - [2.2.2 Policy Gradient](#222-policy-gradient)
      - [2.2.3 Actor-critic Network](#223-actor-critic-network)
  - [2.3 Multi-Agent Reinforcement Learning](#23-multi-agent-reinforcement-learning)
  - [2.4 Training and Execution Strategies in MARL](#24-training-and-execution-strategies-in-marl)
      - [2.4.1 Centralized training with decentralized execution](#241-centralized-training-with-decentralized-execution)
      - [2.4.2 Decentralized training with decentralized execution](#242-decentralized-training-with-decentralized-execution)
  - [2.5 MARL Algorithm Variants](#25-marl-algorithm-variants)
      - [2.5.1 Value function decomposition](#251-value-function-decomposition)
      - [2.5.2 Learning to Communicate](#252-learning-to-communicate)
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

1. Scheffer, Tobias, Christian Decomain, and Stefan Wrobel. **"Active hidden markov models for information extraction."** Advances in Intelligent Data Analysis: 4th International Conference, IDA 2001 Cascais, Portugal, September 13–15, 2001 Proceedings 4. Springer Berlin Heidelberg, 2001. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Active+hidden+markov+models+for+information+extraction&btnG=) [[Paper]](https://link.springer.com/chapter/10.1007/3-540-44816-0_31)  ![]

2. Houlsby, Neil, et al. **"Bayesian active learning for classification and preference learning."** arXiv preprint arXiv:1112.5745 (2011). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Bayesian+active+learning+for+classification+and+preference+learning&btnG=) [[Paper]](https://arxiv.org/pdf/1112.5745.pdf)  ![]

3. Gal, Yarin, Riashat Islam, and Zoubin Ghahramani. **"Deep bayesian active learning with image data."**  International conference on machine learning. PMLR, 2017. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Deep+bayesian+active+learning+with+image+data&btnG=) [[Paper]](http://proceedings.mlr.press/v70/gal17a/gal17a.pdf)  ![]

4. Gal, Yarin, and Zoubin Ghahramani.  **"Bayesian convolutional neural networks with Bernoulli approximate variational inference."** arXiv preprint arXiv:1506.02158 (2015). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Bayesian+convolutional+neural+networks+with+bernoulli+approximate+variational+inference&btnG=) [[Paper]](https://arxiv.org/pdf/1506.02158.pdf) 

5. Haussmann, Manuel, Fred A. Hamprecht, and Melih Kandemir. **"Deep active learning with adaptive acquisition."** arXiv preprint arXiv:1906.11471 (2019). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Deep+active+learning+with+adaptive+acquisition&btnG=) [[Paper]](https://arxiv.org/pdf/1906.11471.pdf)  [[Code]](https://github.com/manuelhaussmann/ral)

6. Geifman, Yonatan, and Ran El-Yaniv. **"Deep active learning with a neural architecture search."** Advances in Neural Information Processing Systems 32 (2019). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Deep+active+learning+with+a+neural+architecture+search&btnG=) [[Paper]](https://proceedings.neurips.cc/paper/2019/file/b59307fdacf7b2db12ec4bd5ca1caba8-Paper.pdf) 


#### 2.4.2 Decentralized training with decentralized execution (DTDE)

1. Lee, Dong-Hyun.  **"Pseudo-label: The simple and efficient semi-supervised learning method for deep neural networks."** Workshop on challenges in representation learning, ICML. Vol. 3. No. 2. 2013. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Pseudo-label%3A+The+simple+and+efficient+semi-supervised+learning+method+for+deep+neural+networks&btnG=) [[Paper]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Pseudo-label%3A+The+simple+and+efficient+semi-supervised+learning+method+for+deep+neural+networks&btnG=) [[Code]](https://github.com/iBelieveCJM/pseudo_label-pytorch) 

2. Xie, Qizhe, et al. **"Self-training with noisy student improves imagenet classification."** Proceedings of the IEEE/CVF conference on computer vision and pattern recognition. 2020. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Self-training+with+noisy+student+improves+imagenet+classification.&btnG=) [[Paper]](https://openaccess.thecvf.com/content_CVPR_2020/papers/Xie_Self-Training_With_Noisy_Student_Improves_ImageNet_Classification_CVPR_2020_paper.pdf)  [[Code]](https://github.com/google-research/noisystudent)  

3. Liu, Yen-Cheng, et al. **"Unbiased teacher for semi-supervised object detection."**  arXiv preprint arXiv:2102.09480 (2021). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Unbiased+teacher+for+semi-supervised+object+detection&btnG=) [[Paper]](https://arxiv.org/pdf/2102.09480.pdf)  [[Code]](https://github.com/facebookresearch/unbiased-teacher) 

4. Tarvainen, Antti, and Harri Valpola. **"Mean teachers are better role models: Weight-averaged consistency targets improve semi-supervised deep learning results."** Advances in neural information processing systems 30 (2017). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Mean+teachers+are+better+role+models%3A+Weightaveraged+consistency+targets+improve+semi-supervised+deep+learning+results&btnG=) [[Paper]](https://proceedings.neurips.cc/paper/2017/file/68053af2923e00204c3ca7c6a3150cf7-Paper.pdf)  [[Code]](https://github.com/CuriousAI/mean-teacher)  

5. Zhou, Zhi-Hua. **"When semi-supervised learning meets ensemble learning."** Frontiers of Electrical and Electronic Engineering in China 6 (2011): 6-16. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=When+semi-supervised+learning+meets+ensemble+learning&btnG=) [[Paper]](https://link.springer.com/content/pdf/10.1007/s11460-011-0126-2.pdf) 

6. Zhou, Zhi-Hua. **"Ensemble methods: foundations and algorithms."** CRC press, 2012. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Ensemble+methods%3A+foundations+and+algorithms&btnG=) [[Paper]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Ensemble+methods%3A+foundations+and+algorithms&btnG=) 

7. Bennett, Kristin, and Ayhan Demiriz. **"Semi-supervised support vector machines."** Advances in Neural Information processing systems 11 (1998). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Semi-supervised+support+vector+machines&btnG=) [[Paper]](https://proceedings.neurips.cc/paper/1998/file/b710915795b9e9c02cf10d6d2bdb688c-Paper.pdf)

8. Ben-David, Shai, et al. **"Learning low density separators."** Artificial Intelligence and Statistics. PMLR, 2009. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Learning+low+density+separators&btnG=) [[Paper]](http://proceedings.mlr.press/v5/ben-david09a/ben-david09a.pdf)  [[Code]]()  

9. Li, Yu-Feng, et al. **"Convex and scalable weakly labeled SVMs."** Journal of Machine Learning Research 14.7 (2013). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Convex+and+scalable+weakly+labeled+svms&btnG=) [[Paper]](https://www.jmlr.org/papers/volume14/li13a/li13a.pdf) 

10. Chapelle, Olivier, Vikas Sindhwani, and Sathiya S. Keerthi. **"Optimization techniques for semi-supervised support vector machines."** Journal of Machine Learning Research 9.2 (2008). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Optimization+techniques+for+semi-supervised+support+vector+machines&btnG=) [[Paper]](https://www.jmlr.org/papers/volume9/chapelle08a/chapelle08a.pdf) 


### 2.5 MARL Algorithm Variants

#### 2.5.1 Value function decomposition

1. Andrews, Stuart, Ioannis Tsochantaridis, and Thomas Hofmann. **"Support vector machines for multiple-instance learning."** Advances in neural information processing systems 15 (2002). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=+Support+vector+machines+for+multiple-instance+learning&btnG=) [[Paper]](https://proceedings.neurips.cc/paper/2002/file/3e6260b81898beacda3d16db379ed329-Paper.pdf) 

2. Wu, Jiajun, et al. **"Deep multiple instance learning for image classification and auto-annotation."** Proceedings of the IEEE conference on computer vision and pattern recognition. 2015.  [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Deep+multiple+instance+learning+for+image+classification+and+auto-annotation.&btnG=) [[Paper]](https://openaccess.thecvf.com/content_cvpr_2015/html/Wu_Deep_Multiple_Instance_2015_CVPR_paper.html) 

3. Ilse, Maximilian, Jakub Tomczak, and Max Welling. **"Attention-based deep multiple instance learning."** International conference on machine learning. PMLR, 2018. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Attention-based+deep+multiple+instance+learning&btnG=) [[Paper]](http://proceedings.mlr.press/v80/ilse18a/ilse18a.pdf) 


#### 2.5.2 Learning to Communicate

1. Caron, Mathilde, et al. **"Deep clustering for unsupervised learning of visual features."** Proceedings of the European conference on computer vision (ECCV). 2018. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Deep+clustering+for+unsupervised+learning+of+visual+features.&btnG=) [[Paper]](https://openaccess.thecvf.com/content_ECCV_2018/papers/Mathilde_Caron_Deep_Clustering_for_ECCV_2018_paper.pdf) 

2. Yang, Jianwei, Devi Parikh, and Dhruv Batra. **"Joint unsupervised learning of deep representations and image clusters."** Proceedings of the IEEE conference on computer vision and pattern recognition. 2016. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Joint+unsupervised+learning+of+deep+representations+and+image+clusters.&btnG=) [[Paper]](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Yang_Joint_Unsupervised_Learning_CVPR_2016_paper.pdf)  [[Code]](https://github.com/jwyang/JULE.torch) 

3. Xie, Junyuan, Ross Girshick, and Ali Farhadi. **"Unsupervised deep embedding for clustering analysis."** International conference on machine learning. PMLR, 2016. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Unsupervised+deep+embedding+for+clustering+analysis&btnG=) [[Paper]](http://proceedings.mlr.press/v48/xieb16.pdf) 

4. Noroozi, Mehdi, et al. **"Boosting self-supervised learning via knowledge transfer."** Proceedings of the IEEE conference on computer vision and pattern recognition. 2018. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Boosting+selfsupervised+learning+via+knowledge+transfer.+&btnG=) [[Paper]](https://openaccess.thecvf.com/content_cvpr_2018/papers/Noroozi_Boosting_Self-Supervised_Learning_CVPR_2018_paper.pdf) 

5. Tian, Yonglong, Dilip Krishnan, and Phillip Isola. **"Contrastive multiview coding."** Computer Vision–ECCV 2020: 16th European Conference, Glasgow, UK, August 23–28, 2020, Proceedings, Part XI 16. Springer International Publishing, 2020. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Contrastive+multiview+coding.&btnG=) [[Paper]](https://arxiv.org/pdf/1906.05849.pdf) [[Code]](https://github.com/HobbitLong/CMC/)

6. Caron, Mathilde, et al. **"Unsupervised learning of visual features by contrasting cluster assignments."** Advances in neural information processing systems 33 (2020): 9912-9924. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Unsupervised+learning+of+visual+features+by+contrasting+cluster+assignments.+&btnG=) [[Paper]](https://proceedings.neurips.cc/paper/2020/file/70feb62b69f16e0238f741fab228fec2-Paper.pdf) [[Code]](https://github.com/facebookresearch/swav) 


#### 2.5.3 Hierarchical structure
1. Arthur, David, and Sergei Vassilvitskii. **"K-means++ the advantages of careful seeding."** Proceedings of the eighteenth annual ACM-SIAM symposium on Discrete algorithms. 2007. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=K-means%2B%2B+the+advantages+of+careful+seeding&btnG=) [[Paper]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=K-means%2B%2B+the+advantages+of+careful+seeding&btnG=) 

2. Yang, Jianwei, Devi Parikh, and Dhruv Batra. "Joint unsupervised learning of deep representations and image clusters." Proceedings of the IEEE conference on computer vision and pattern recognition. 2016. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Joint+unsupervised+learning+of+deep+representations+and+image+clusters&btnG=) [[Paper]](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Yang_Joint_Unsupervised_Learning_CVPR_2016_paper.pdf) [[Code]](https://github.com/jwyang/JULE.torch) 

3. Ji, Zeguang, et al. "SEDLNet: An unsupervised precise lightweight extraction method for farmland areas." Computers and Electronics in Agriculture 210 (2023): 107886.  [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=SEDLNet%3A+An+unsupervised+precise+lightweight+extraction+method+for+farmland+areas&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169923002740)

#### 2.5.4 Causal inference


## 3. 🤖 Towards applications in connected and autonomous vehicles


### 3.1 One-dimensional Cooperation

Instructions are used in various human-computer interaction (HCI) tasks, such as virtual assistants, chatbots, etc. 

1. Coletta, Luiz FS, et al. **"Novelty detection in UAV images to identify emerging threats in eucalyptus crops."** Computers and Electronics in Agriculture 196 (2022): 106901. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Novelty+detection+in+UAV+images+to+identify+emerging+threats+in+eucalyptus+crops&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169922002186?casa_token=ZFhy1QK7aakAAAAA:wI-NrE3CAa8ph4hZ_iuU-qB0hXz6c6Kpn4f5P301ZI7qxFC4R6mxiOOogDMET4qBwo8zhARxUnE)  

2. Bollis, Edson, et al. **"Weakly supervised attention-based models using activation maps for citrus mite and insect pest classification."** Computers and Electronics in Agriculture 195 (2022): 106839. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Weakly+supervised+attention-based+models+using+activation+maps+for+citrus+mite+and+insect+pest+classification&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169922001569?casa_token=ELjQTHzpJpIAAAAA:7o5dvi6KmPG3KBoC1EfUSdwb544-Gr9c2SUrhMoIJEx2OQzDMX9vhRMRpyMCk8pIJ5hPgRMu8ME)  

3. Monowar, Muhammad Mostafa, et al. **"Self-Supervised Clustering for Leaf Disease Identification."** Agriculture 12.6 (2022): 814. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Self-Supervised+Clustering+for+Leaf+Disease+Identification&btnG=) [[Paper]](https://www.mdpi.com/2077-0472/12/6/814)  

4. Kim, Taejoo, et al. **"Instance-Aware Plant Disease Detection by Utilizing Saliency Map and Self-Supervised Pre-Training."** Agriculture 12.8 (2022): 1084. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Instance-Aware+Plant+Disease+Detection+by+Utilizing+Saliency+Map+and+Self-Supervised+Pre-Training&btnG=) [[Paper]](https://www.mdpi.com/2077-0472/12/8/1084)  

5. Li, Yang, and Xuewei Chao. **"Semi-supervised few-shot learning approach for plant diseases recognition."** Plant Methods 17 (2021): 1-10. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Semi-supervised+few-shot+learning+approach+for+plant+diseases+recognition&btnG=) [[Paper]](https://link.springer.com/article/10.1186/s13007-021-00770-1) 

 


### 3.2 Two-dimensional Cooperation

1. Marszalek, Michael L., et al. **"Self-supervised learning--A way to minimize time and effort for precision agriculture?."** arXiv preprint arXiv:2204.02100 (2022). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Self-supervised+learning--A+way+to+minimize+time+and+effort+for+precision+agriculture%3F&btnG=) [[Paper]](https://arxiv.org/abs/2204.02100) 

2. Yang, Yana, et al. **"Dissimilarity-based active learning for embedded weed identification."** Turkish Journal of Agriculture and Forestry 46.3 (2022): 390-401. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Dissimilarity-based+active+learning+for+embedded+weed+identification&btnG=) [[Paper]](https://journals.tubitak.gov.tr/agriculture/vol46/iss3/11/) 

3. Nong, Chunshi, Xijian Fan, and Junling Wang. **"Semi-supervised Learning for Weed and Crop Segmentation Using UAV Imagery."** Frontiers in Plant Science 13 (2022). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Semi-supervised+Learning+for+Weed+and+Crop+Segmentation+Using+UAV+Imagery&btnG=) [[Paper]](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9283949/)  

4. Güldenring, Ronja, and Lazaros Nalpantidis. **"Self-supervised contrastive learning on agricultural images."** Computers and Electronics in Agriculture 191 (2021): 106510. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Self-supervised+contrastive+learning+on+agricultural+images&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169921005275)  

5. Shorewala, Shantam, et al. **"Weed density and distribution estimation for precision agriculture using semi-supervised learning."** IEEE access 9 (2021): 27971-27986. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Weed+Density+and+Distribution+Estimation+for+Precision+Agriculture+Using+Semi-Supervised+Learning&btnG=) [[Paper]](https://ieeexplore.ieee.org/abstract/document/9350244) 

6. Hu, Chengsong, J. Alex Thomasson, and Muthukumar V. Bagavathiannan. **"A powerful image synthesis and semi-supervised learning pipeline for site-specific weed detection."** Computers and Electronics in Agriculture 190 (2021): 106423. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+powerful+image+synthesis+and+semi-supervised+learning+pipeline+for+site-specific+weed+detection&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169921004403?casa_token=qbLLY8XNSGoAAAAA:Xo4rcwElVN_SDaVDNPJLekHBVcgRx9tb7TMKXFsfmKT_Az3LXq9ewaCHCx2MMhDl0MDBNJYnH5A)  
  

### 3.3 Three-dimensional Cooperation

#### 3.3.1 Traffic signal control
1. Mofan Zhou, et al. **"Development of an efficient driving strategy for connected and automated vehicles at signalized intersections: A reinforcement learning approach."** Computers and Electronics in Agriculture 205 (2023): 107624. [[Google Scholar]](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=Development+of+an+efficient+driving+strategy+for+connected+and+automated+vehicles+at+signalized+intersections%3A+A+reinforcement+learning+approach&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8848852)  

2. Bhattarai, Uddhav, and Manoj Karkee. **"A weakly-supervised approach for flower/fruit counting in apple orchards."** Computers in Industry 138 (2022): 103635. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+weakly-supervised+approach+for+flower%2Ffruit+counting+in+apple+orchards&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0166361522000306?casa_token=xWeCzyeEZZUAAAAA:LUjMhynGwwsck4eA-rHwfmSlEPYmSr8BRLwiSdyYLfCRMzt-jS6akIiGCRBnNR7ccLM8pcKeVLQ)  

3. Bellocchio, Enrico, et al. **"A novel vision-based weakly supervised framework for autonomous yield estimation in agricultural applications."** Engineering Applications of Artificial Intelligence 109 (2022): 104615. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+novel+vision-based+weakly+supervised+framework+for+autonomous+yield+estimation+in+agricultural+applications&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0952197621004310?casa_token=-9FqEhV_TIwAAAAA:FsWlWxH_tdGfZ-R2BoinYcHee6s-vxMjNIu-yPkv-qE7C6DGpXN4qA-s_o-tNPNvJwA2rX_Dk7U)  

4. Casado-García, A., et al. **"Semi-supervised deep learning and low-cost cameras for the semantic segmentation of natural images in viticulture."** Precision Agriculture (2022): 1-26. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Semi-supervised+deep+learning+and+low-cost+cameras+for+the+semantic+segmentation+of+natural+images+in+viticulture&btnG=) [[Paper]](https://link.springer.com/article/10.1007/s11119-022-09929-9)  

5. Khaki, Saeed, et al. **"Deepcorn: A semi-supervised deep learning method for high-throughput image-based corn kernel counting and yield estimation."** Knowledge-Based Systems 218 (2021): 106874. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=DeepCorn%3A+A+semi-supervised+deep+learning+method+for+high-throughput+image-based+corn+kernel+counting+and+yield+estimation&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0950705121001374?casa_token=l6_EWtXTZKYAAAAA:-66kxmrbl64ho7xiOI12o2fopzjHy83TQznz_hYZDktYp13qRlEysM2kepX2eUVaiiI0FlJheuU)  

6. Bellocchio, Enrico, et al. **"Combining domain adaptation and spatial consistency for unseen fruits counting: a quasi-unsupervised approach."** IEEE Robotics and Automation Letters 5.2 (2020): 1079-1086. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Combining+domain+adaptation+and+spatial+consistency+for+unseen+fruits+counting%3A+A+quasi+unsupervised+approach&btnG=) [[Paper]](https://ieeexplore.ieee.org/abstract/document/8957569?casa_token=KMOqwa2X0x8AAAAA:Wnywsh46mUKKU8D_8U_HY3JLODoA2MYFGzGqA7k3MLGXNVXKSR4Nh8kaXjj9LHNEe3GHpU2zsiw)  

7. Bellocchio, Enrico, et al. **"Weakly supervised fruit counting for yield estimation using spatial consistency."** IEEE Robotics and Automation Letters 4.3 (2019): 2348-2355. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Weakly+Supervised+Fruit+Counting+for+Yield+Estimation+Using+Spatial+Consistency&btnG=) [[Paper]](https://ieeexplore.ieee.org/abstract/document/8661632?casa_token=JCFKLG19GCwAAAAA:TRJtK24bhVT51_jKh3pODODsooRuiimzF_6uKq7LbgmuyFtVkKv_q7gAsoTKcdfTdgGyfMTSQ5M) 

8. Roy, Pravakar, et al. **"Vision-based preharvest yield mapping for apple orchards."** Computers and Electronics in Agriculture 164 (2019): 104897. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Vision-based+preharvest+yield+mapping+for+apple+orchards&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169919303436?casa_token=0cpG4d1hc50AAAAA:LysqbihEr3zY5-2Ub7zl878HhgwHCQgzOt5wysTou9B1bKXdXxxkkcr2rZBVXgfku30onUkaCZE)  

#### 3.3.2 On-ramps merging

1. Kong, Qingchen, et al. **"A recurrent network based on active learning for the assessment of fish feeding status."** Computers and Electronics in Agriculture 198 (2022): 106979. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+recurrent+network+based+on+active+learning+for+the+assessment+of+fish+feeding+status&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169922002964?casa_token=3sEdz3v21LgAAAAA:Xt0sn8l-FcWHyTSPuTPg-zR1nIkH59hhu0yl2uju8z2kDi2yjGVYfIo-egNbffOruatbiO4C6Qw)  


#### 3.3.3 Unsignalized intersections

1. Lin, Xufeng, et al. **"Self-Supervised Leaf Segmentation under Complex Lighting Conditions."** Pattern Recognition 135 (2023): 109021. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Self-Supervised+Leaf+Segmentation+under+Complex+Lighting+Conditions&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0031320322005015?casa_token=hbczlttXx3QAAAAA:Sj_D4jBQEBfVQpM2H1V3KTVqvFyzz1rvErGPqMFFIdVWSqiJMJMYONoWnRHGONStKrc4p-Vt0oM)  [[Code]](https://github.com/lxfhfut/Self-Supervised-Leaf-Segmentation) 

2. Tschand, Arya. **"Semi-supervised machine learning analysis of crop color for autonomous irrigation."** Smart Agricultural Technology 3 (2023): 100116. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Semi-Supervised+Machine+Learning+Analysis+of+Crop+Color+for+Autonomous+Irrigation&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S2772375522000818) 

3. Blok, Pieter M., et al. **"Active learning with MaskAL reduces annotation effort for training Mask R-CNN on a broccoli dataset with visually similar classes."** Computers and Electronics in Agriculture 197 (2022): 106917. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Active+learning+with+MaskAL+reduces+annotation+effort+for+training+Mask+R-CNN+on+a+broccoli+dataset+with+visually+similar+classes&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169922002344) [[Code]](https://github.com/pieterblok/maskal) 

4. Rawat, Shivangana, et al. **"How Useful Is Image-Based Active Learning for Plant Organ Segmentation?."** Plant Phenomics 2022 (2022). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=How+Useful+Is+Image-Based+Active+Learning+for+Plant+Organ+Segmentation%3F&btnG=) [[Paper]](https://downloads.spj.sciencemag.org/plantphenomics/2022/9795275.pdf)   

5. Li, Lei, et al. **"Leaf vein segmentation with self-supervision."** Computers and Electronics in Agriculture 203 (2022): 107352. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Leaf+vein+segmentation+with+self-supervision&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169922006603?casa_token=DgMIEFP-89YAAAAA:8nAwxkwH7QDAPJutUAtUdWe0vmWvwB2apcT1huH4tRQLAQF1ml2B_2h0mIrHOujVsLoiSTJsZi0)  

6. Zhang, Xin, et al. **"The Self-Supervised Spectral–Spatial Vision Transformer Network for Accurate Prediction of Wheat Nitrogen Status from UAV Imagery."** Remote Sensing 14.6 (2022): 1400. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=The+Self-Supervised+Spectral%E2%80%93Spatial+Vision+Transformer+Network+for+Accurate+Prediction+of+Wheat+Nitrogen+Status+from+UAV+Imagery&btnG=) [[Paper]](https://www.mdpi.com/2072-4292/14/6/1400)  



#### 3.3.4 Simulation Platforms
1. Liu, Yisen, et al. **"Joint optimization of autoencoder and self-supervised classifier: anomaly detection of strawberries using hyperspectral imaging."** Computers and Electronics in Agriculture 198 (2022): 107007. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Joint+optimization+of+autoencoder+and+Self-Supervised+Classifier%3A+Anomaly+detection+of+strawberries+using+hyperspectral+imaging&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169922003246?casa_token=mbiSlzaiRvEAAAAA:6rfTcrs7MG1etkv2cGSz75ZfjBAUc0OdCa5l32TvDYmXNrqJ2iRcbNjC4Ee-F-rq4L0bLx3gz_4)  

2. Li, Weitao, et al. **"Greengage grading using stochastic configuration networks and a semi-supervised feedback mechanism."** Information Sciences 488 (2019): 1-12. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Greengage+grading+using+stochastic+configuration+networks+and+a+semi-supervised+feedback+mechanism&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0020025519301501?casa_token=n_LudCJnoLQAAAAA:8OxTDeg7i8axhkrkSPksjPHqHKj_ecmbVXDEFqQaipZJ7z8FAOeptHb03E-Wzw2KUCvvjZwjz4M) 

3. Marino, Sofia, Pierre Beauseroy, and André Smolarz. **"Weakly-supervised learning approach for potato defects segmentation."** Engineering Applications of Artificial Intelligence 85 (2019): 337-346. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Weakly-supervised+learning+approach+for+potato+defects+segmentation&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0952197619301630?casa_token=M83Hltqn6dkAAAAA:T-gCy-NLjAKyuIeu-b2ccq_b9xYK9UTKkg1VOgF49C_1mz51bI5YIkThmkb6Hnly7Q4KUjW-aXU)  


<!-- TODO: tweets & slides? -->

---

<!-- omit in toc -->
