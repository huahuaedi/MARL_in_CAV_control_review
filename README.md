<!-- omit in toc -->
# Awesome Label-Efficient Learning in Agricutlture: A Comprehensive Review


[![Awesome](https://awesome.re/badge.svg)](https://github.com/DongChen06/Label-efficient-in-Agriculture
) ![](https://img.shields.io/github/stars/DongChen06/Label-efficient-in-Agriculture?style=social)

![](https://img.shields.io/github/last-commit/DongChen06/Label-efficient-in-Agriculture?color=#00FA9A) ![](https://img.shields.io/badge/PaperNumber-70-blue) ![](https://img.shields.io/badge/PRs-Welcome-red) 

A curated list of awesome **Label-efficient Learning in Agricutlture** papers 🔥🔥🔥. 

Currently maintained by <ins>[Jiajia Li](xx) @ MSU</ins> and <ins>[Dong Chen](https://scholar.google.com/citations?user=dwvTqeUAAAAJ&hl=en) @ MSU</ins>. 


**<font color='red'>Work still in progress</font>**  🚀, **we appreciate any suggestions and contributions** ❤️.

---

<!-- What is instruction learning?
Why instruction learning?
-->

<!-- TODO
## Our scope:
We aim to stay up-to-date with the most innovative developments in the field and gain valuable insights into the future of instruction-learning technology.👀 organize a systematic and comprehensive overview of instructional learning.

1. Stay up-to-date with the most innovative developments in this field.
2. Gain valuable insights into the future of instruction-learning technology.
3. 
-->


<!-- omit in toc -->
## How to contribute?

If you have any suggestions or find any missed papers, feel free to reach out or submit a [pull request](https://github.com/DongChen06/Label-efficient-in-Agriculture/pulls):

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

```
@article{li2023label,
  title={Label-Efficient Learning in Agriculture: A Comprehensive Review},
  author={Li, Jiajia and Chen, Dong and Qi, Xinda and Li, Zhaojian and Huang, Yanbo and Morris, Daniel and Tan, Xiaobo},
  journal={arXiv preprint arXiv:2305.14691},
  year={2023}
}
```

<!-- TODO: add survey citation and link -->

<!-- omit in toc -->
## 🔍 Table of Contents 

- [1. 💁🏽‍♀️ Introduction](#1-️-introduction)
- [2. 🎓 Surveys and Tutorials](#2--surveys-and-tutorials)
- [3. 🗂️ Taxonomy](#3-️-taxonomy)
  - [3.1 Weak Supervision](#31-weak-supervision)
      - [3.1.1 Active learning](#311-active-learning)
      - [3.1.2 Semi-supervised learning](#312-semi-supervised-learning)
      - [3.1.3 Weakly-supervised learning](#313-weakly-supervised-learning)
  - [3.2 No supervision](#32-no-supervision)
      - [3.2.1 Self-supervised learning](#321-self-supervised-learning)
      - [3.2.2 Unsupervised representation learning](#322-unsupervised-representation-learning)
- [4. 🤖 Applications](#4--applications)
  - [4.1 Plant health](#41-plant-health)
  - [4.2 Weed and crop management](#42-weed-and-crop-management)
  - [4.3 Fruit detection](#43-fruit-detection)
  - [4.4 Aquaculture](#44-aquaculture)
  - [4.5 Plant Phenotyping](#45-plant-phenotyping)
  - [4.6 Postharvest quality assessment](#46-postharvest-quality-assessment)
- [5. 📚 Corpora](#6--corpora)
- [6. 📖 Extended Reading](#7--extended-reading)
  - [6.1 Instruction Induction](#71-instruction-induction)
  
---


## 1. 💁🏽‍♀️ Introduction



Why label-efficient learning instead of supervised learning?

- 👉 **Affordable.**  For supervised learning, each task usually requires extensive labeled examples 💰. While for instruction learning, each task may require only one instruction and just a few examples 🤩.
- 👉 **One model, all tasks.** An ideal AI system should be able to quickly understand and handle various new tasks 💫.
- 👉 **A promising research direction.** Traditional supervised learning uses labeled instances to represent the task semantics, i.e., training models by observing numerous examples to recover the original task meaning. Therefore, **why not directly use the task instruction**, **which has already occupied the essential task semantics**?

<!-- We all know collecting extensive labeled examples are usually expensive 💰. -->


## 2. 🎓 Surveys and Tutorials

<!-- There are several awesome surveys and tutorials on semi-supervised, active learning, weakly-supervised learning, unsupervised learning, and self-supervised learning, while most of them focus on one of the topic and none of them are focusing on agricutural applications. -->
<!-- To our knowledge, our survey is the first one to provide a comprehensive and broader overview of the field of label-efficient learning. -->
<!-- Since each survey focuses on specific supervision types, we attach a label to each of them to distinguish these topics.
, including `active learning`, `semi-supervised learning`, `weakly supervised leaning`, `self-supervised leaning` and `unsupervised learning` (which means a broader perspective). -->

The following topics are included: ![](https://img.shields.io/badge/-active--learning-brightgreen)
![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)
![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)
![](https://img.shields.io/badge/-self--supervised%20leaning-blue)
![](https://img.shields.io/badge/-unsupervised%20learning-red)
  
1. Zhou, Zhi-Hua. **"A brief introduction to weakly supervised learning."**  National science review 5.1 (2018): 44-53.  [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+brief+introduction+to+weakly+supervised+learning&btnG=) [[Paper]](https://academic.oup.com/nsr/article/5/1/44/4093912) ![](https://img.shields.io/badge/-active--learning-brightgreen) ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)  ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

2. Kääriäinen, Matti. **"Active learning in the non-realizable case."** International Conference on Algorithmic Learning Theory. Springer, Berlin, Heidelberg, 2006.  [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Active+learning+in+the+non-realizable+case&btnG=) [[Paper]](https://link.springer.com/chapter/10.1007/11894841_9)  ![](https://img.shields.io/badge/-active--learning-brightgreen)

3. Schmarje, Lars, et al. **"A survey on semi-, self-and unsupervised learning for image classification."** IEEE Access 9 (2021): 82146-82168.  [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+survey+on+semi-%2C+self-and+unsupervised+learning+for+image+classification&btnG=) [[Paper]](https://ieeexplore.ieee.org/abstract/document/9442775) ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)  ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)  ![](https://img.shields.io/badge/-unsupervised%20learning-red)

4. Jing, Longlong, and Yingli Tian. **"Self-supervised visual feature learning with deep neural networks: A survey."** IEEE transactions on pattern analysis and machine intelligence 43.11 (2020): 4037-4058.  [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Self-supervised+visual+feature+learning+with+deep+neural+networks%3A+A+survey&btnG=) [[Paper]](https://ieeexplore.ieee.org/abstract/document/9086055)  ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)

5. Yan, Jun, and Xiangfeng Wang. **"Unsupervised and semi‐supervised learning: the next frontier in machine learning for plant systems biology."** The Plant Journal (2022).  [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Unsupervised+and+semi%E2%80%90supervised+learning%3A+the+next+frontier+in+machine+learning+for+plant+systems+biology&btnG=) [[Paper]](https://onlinelibrary.wiley.com/doi/full/10.1111/tpj.15905) ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)  ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)  ![](https://img.shields.io/badge/-unsupervised%20learning-red)

6. Van Engelen, Jesper E., and Holger H. Hoos. **"A survey on semi-supervised learning."** Machine Learning 109.2 (2020): 373-440.  [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+survey+on+semi-supervised+learning&btnG=) [[Paper]](https://link.springer.com/article/10.1007/s10994-019-05855-6) ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

7. Fatima, Tazeen, and Tariq Mahmood. **"Semi-Supervised Learning in Smart Agriculture: A Systematic Literature Review."** 2021 6th International Multi-Topic ICT Conference (IMTIC). IEEE, 2021.  [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Semi-Supervised+Learning+in+Smart+Agriculture%3A+A+Systematic+Literature+Review&btnG=) [[Paper]](https://ieeexplore.ieee.org/abstract/document/9719809) ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

8. Sohn, Kihyuk, et al. **"A simple semi-supervised learning framework for object detection."** arXiv preprint arXiv:2005.04757 (2020).  [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+simple+semi-supervised+learning+framework+for+object+detection&btnG=) [[Paper]](https://arxiv.org/abs/2005.04757)  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

9. Shen, Wei, et al. **"A Survey on Label-efficient Deep Segmentation: Bridging the Gap between Weak Supervision and Dense Prediction."** arXiv preprint arXiv:2207.01223 (2022).  [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+Survey+on+Label-efficient+Deep+Segmentation%3A+Bridging+the+Gap+between+Weak+Supervision+and+Dense+Prediction&btnG=) [[Paper]](https://arxiv.org/abs/2207.01223)  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

10. Settles, Burr. **"Active learning literature survey."** University of Wisconsin-Madison Department of Computer Sciences (2009). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Active+learning+literature+survey&btnG=) [[Paper]](https://minds.wisconsin.edu/bitstream/handle/1793/60660/TR1648.pdf?sequence=1)  ![](https://img.shields.io/badge/-active--learning-brightgreen)

11. Ren, Pengzhen, et al. **"A survey of deep active learning."** ACM computing surveys (CSUR) 54.9 (2021): 1-40. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+survey+of+deep+active+learning&btnG=) [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3472291?casa_token=8z8Q0AaEKsgAAAAA:ECSiXZ3Hqo7a4V2g3H99L2zg2X9RcHZtzpuPpwuOSKQCq29pAkYSuFzIRHh2Ix8qYv4UaaNgS7Uc1A)  ![](https://img.shields.io/badge/-active--learning-brightgreen) 

12. Aggarwal, Charu C., et al. **"Active learning: A survey."** Data classification. Chapman and Hall/CRC, 2014. 599-634. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Active+learning%3A+A+survey&btnG=) [[Paper]](https://www.taylorfrancis.com/chapters/edit/10.1201/b17320-27/active-learning-survey-charu-aggarwal-xiangnan-kong-quanquan-gu-jiawei-han-philip-yu)  ![](https://img.shields.io/badge/-active--learning-brightgreen)

13. Chong, Yanwen, et al. **"Graph-based semi-supervised learning: A review."** Neurocomputing 408 (2020): 216-230. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Graph-based+semi-supervised+learning%3A+A+review&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0925231220304938?casa_token=1qMKCz9EAxYAAAAA:uCWWy2guGQ7C8XUByKSVeSA9wvY1jhpYqKDBYeae6pv5tRBRCCZ3s_mTu7o5TzBf-2YdsZxd0ok) ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

14. Shen, Wei, et al.  **"A survey on label-efficient deep image segmentation: Bridging the gap between weak supervision and dense prediction. "**  IEEE Transactions on Pattern Analysis and Machine Intelligence (2023). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+survey+on+label-efficient+deep+image+segmentation%3A+Bridging+the+gap+between+weak+supervision+and+dense+prediction&btnG=) [[Paper]](https://arxiv.org/pdf/2207.01223.pdf) ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)  ![](https://img.shields.io/badge/-unsupervised%20learning-red) ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

15. Foulds, James, and Eibe Frank. **"A review of multi-instance learning assumptions."** The knowledge engineering review 25.1 (2010): 1-25. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+review+of+multi-instance+learning+assumptions&btnG=) [[Paper]](https://www.cambridge.org/core/services/aop-cambridge-core/content/view/0915098C83BF119A377015A45952247A/S026988890999035Xa.pdf/a-review-of-multi-instance-learning-assumptions.pdf) ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

16. Carbonneau, Marc-André, et al. **"Multiple instance learning: A survey of problem characteristics and applications."** Pattern Recognition 77 (2018): 329-353. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Multiple+instance+learning%3A+A+survey+of+problem+characteristics+and+applications.&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0031320317304065?casa_token=-E9KP7nrtTcAAAAA:4Wy2HGEpGroKeBWYuquGPhMHkUgvdNJ1y-UmHA77oJPhWz5YWptMu_auRTE1m3VsiJ3OH_cFHpI) ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

17. Chicco, Davide. **"Siamese neural networks: An overview."** Artificial neural networks (2021): 73-94. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Siamese+neural+networks%3A+An+overview.&btnG=) [[Paper]](https://link.springer.com/protocol/10.1007/978-1-0716-0826-5_3) ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)

18. Aljalbout, Elie, et al. **"Clustering with deep learning: Taxonomy and new methods."** arXiv preprint arXiv:1801.07648 (2018). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=+Clustering+with+deep+learning%3A+Taxonomy+and+new+methods&btnG=) [[Paper]](https://arxiv.org/pdf/1801.07648.pdf].) ![](https://img.shields.io/badge/-unsupervised%20learning-red)


## 3. 🗂️ Taxonomy

In our paper, we divide the textual instructions into three categories.

### 3.1 Weak Supervision

#### 3.1.1 Active learning

1. Scheffer, Tobias, Christian Decomain, and Stefan Wrobel. **"Active hidden markov models for information extraction."** Advances in Intelligent Data Analysis: 4th International Conference, IDA 2001 Cascais, Portugal, September 13–15, 2001 Proceedings 4. Springer Berlin Heidelberg, 2001. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Active+hidden+markov+models+for+information+extraction&btnG=) [[Paper]](https://link.springer.com/chapter/10.1007/3-540-44816-0_31)  ![](https://img.shields.io/badge/-active--learning-brightgreen)

2. Houlsby, Neil, et al. **"Bayesian active learning for classification and preference learning."** arXiv preprint arXiv:1112.5745 (2011). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Bayesian+active+learning+for+classification+and+preference+learning&btnG=) [[Paper]](https://arxiv.org/pdf/1112.5745.pdf)  ![](https://img.shields.io/badge/-active--learning-brightgreen)

3. Gal, Yarin, Riashat Islam, and Zoubin Ghahramani. **"Deep bayesian active learning with image data."**  International conference on machine learning. PMLR, 2017. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Deep+bayesian+active+learning+with+image+data&btnG=) [[Paper]](http://proceedings.mlr.press/v70/gal17a/gal17a.pdf)  ![](https://img.shields.io/badge/-active--learning-brightgreen)

4. Gal, Yarin, and Zoubin Ghahramani.  **"Bayesian convolutional neural networks with Bernoulli approximate variational inference."** arXiv preprint arXiv:1506.02158 (2015). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Bayesian+convolutional+neural+networks+with+bernoulli+approximate+variational+inference&btnG=) [[Paper]](https://arxiv.org/pdf/1506.02158.pdf) ![](https://img.shields.io/badge/-active--learning-brightgreen)

5. Haussmann, Manuel, Fred A. Hamprecht, and Melih Kandemir. **"Deep active learning with adaptive acquisition."** arXiv preprint arXiv:1906.11471 (2019). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Deep+active+learning+with+adaptive+acquisition&btnG=) [[Paper]](https://arxiv.org/pdf/1906.11471.pdf)  [[Code]](https://github.com/manuelhaussmann/ral) ![](https://img.shields.io/badge/-active--learning-brightgreen)

6. Geifman, Yonatan, and Ran El-Yaniv. **"Deep active learning with a neural architecture search."** Advances in Neural Information Processing Systems 32 (2019). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Deep+active+learning+with+a+neural+architecture+search&btnG=) [[Paper]](https://proceedings.neurips.cc/paper/2019/file/b59307fdacf7b2db12ec4bd5ca1caba8-Paper.pdf)  ![](https://img.shields.io/badge/-active--learning-brightgreen)

#### 3.1.2 Semi-supervised learning

1. Lee, Dong-Hyun.  **"Pseudo-label: The simple and efficient semi-supervised learning method for deep neural networks."** Workshop on challenges in representation learning, ICML. Vol. 3. No. 2. 2013. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Pseudo-label%3A+The+simple+and+efficient+semi-supervised+learning+method+for+deep+neural+networks&btnG=) [[Paper]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Pseudo-label%3A+The+simple+and+efficient+semi-supervised+learning+method+for+deep+neural+networks&btnG=) [[Code]](https://github.com/iBelieveCJM/pseudo_label-pytorch) ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

2. Xie, Qizhe, et al. **"Self-training with noisy student improves imagenet classification."** Proceedings of the IEEE/CVF conference on computer vision and pattern recognition. 2020. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Self-training+with+noisy+student+improves+imagenet+classification.&btnG=) [[Paper]](https://openaccess.thecvf.com/content_CVPR_2020/papers/Xie_Self-Training_With_Noisy_Student_Improves_ImageNet_Classification_CVPR_2020_paper.pdf)  [[Code]](https://github.com/google-research/noisystudent)  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

3. Liu, Yen-Cheng, et al. **"Unbiased teacher for semi-supervised object detection."**  arXiv preprint arXiv:2102.09480 (2021). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Unbiased+teacher+for+semi-supervised+object+detection&btnG=) [[Paper]](https://arxiv.org/pdf/2102.09480.pdf)  [[Code]](https://github.com/facebookresearch/unbiased-teacher)  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

4. Tarvainen, Antti, and Harri Valpola. **"Mean teachers are better role models: Weight-averaged consistency targets improve semi-supervised deep learning results."** Advances in neural information processing systems 30 (2017). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Mean+teachers+are+better+role+models%3A+Weightaveraged+consistency+targets+improve+semi-supervised+deep+learning+results&btnG=) [[Paper]](https://proceedings.neurips.cc/paper/2017/file/68053af2923e00204c3ca7c6a3150cf7-Paper.pdf)  [[Code]](https://github.com/CuriousAI/mean-teacher)  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

5. Zhou, Zhi-Hua. **"When semi-supervised learning meets ensemble learning."** Frontiers of Electrical and Electronic Engineering in China 6 (2011): 6-16. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=When+semi-supervised+learning+meets+ensemble+learning&btnG=) [[Paper]](https://link.springer.com/content/pdf/10.1007/s11460-011-0126-2.pdf)  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

6. Zhou, Zhi-Hua. **"Ensemble methods: foundations and algorithms."** CRC press, 2012. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Ensemble+methods%3A+foundations+and+algorithms&btnG=) [[Paper]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Ensemble+methods%3A+foundations+and+algorithms&btnG=)  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

7. Bennett, Kristin, and Ayhan Demiriz. **"Semi-supervised support vector machines."** Advances in Neural Information processing systems 11 (1998). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Semi-supervised+support+vector+machines&btnG=) [[Paper]](https://proceedings.neurips.cc/paper/1998/file/b710915795b9e9c02cf10d6d2bdb688c-Paper.pdf) ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

8. Ben-David, Shai, et al. **"Learning low density separators."** Artificial Intelligence and Statistics. PMLR, 2009. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Learning+low+density+separators&btnG=) [[Paper]](http://proceedings.mlr.press/v5/ben-david09a/ben-david09a.pdf)  [[Code]]()  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

9. Li, Yu-Feng, et al. **"Convex and scalable weakly labeled SVMs."** Journal of Machine Learning Research 14.7 (2013). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Convex+and+scalable+weakly+labeled+svms&btnG=) [[Paper]](https://www.jmlr.org/papers/volume14/li13a/li13a.pdf) ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

10. Chapelle, Olivier, Vikas Sindhwani, and Sathiya S. Keerthi. **"Optimization techniques for semi-supervised support vector machines."** Journal of Machine Learning Research 9.2 (2008). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Optimization+techniques+for+semi-supervised+support+vector+machines&btnG=) [[Paper]](https://www.jmlr.org/papers/volume9/chapelle08a/chapelle08a.pdf) ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

11. Liu, Wei, Jun Wang, and Shih-Fu Chang. **"Robust and scalable graph-based semisupervised learning."** Proceedings of the IEEE 100.9 (2012): 2624-2638. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Robust+and+scalable+graph-based+semisupervised+learning&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=6235979&casa_token=vp1ZsX-HUWIAAAAA:ANYvFEh5y1bokr2V6DgjMoqUR_HDvIX0LDrg1zO6xxtHhQFMUtz_8WxsuKu1O88F9xDeC-fRZk0&tag=1) ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

12. Liu, Xiao, et al. **"Random forest construction with robust semisupervised node splitting."** IEEE Transactions on Image Processing 24.1 (2014): 471-483. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Random+forest+construction+with+robust+semisupervised+node+splitting.&btnG=) [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=6975199&casa_token=PN8A1ZZ81gsAAAAA:NA_xF889mwDiaOe8Qjptvx-QbqcCYuTKpaPrWFUWxdcMQcEZbgTLcIUE109Fh2CqocHzGA9Gwco&tag=1) ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

13. Fu, Yinkai, et al. **"Semi-supervised segmentation of multi-scale soil pores based on a novel receptive field structure."** Computers and Electronics in Agriculture 212 (2023): 108071. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Semi-supervised+segmentation+of+multi-scale+soil+pores+based+on+a+novel+receptive+field+structure&btnG=)  [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169923004593)

#### 3.1.3 Weakly supervised learning
1. Andrews, Stuart, Ioannis Tsochantaridis, and Thomas Hofmann. **"Support vector machines for multiple-instance learning."** Advances in neural information processing systems 15 (2002). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=+Support+vector+machines+for+multiple-instance+learning&btnG=) [[Paper]](https://proceedings.neurips.cc/paper/2002/file/3e6260b81898beacda3d16db379ed329-Paper.pdf) ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

2. Wu, Jiajun, et al. **"Deep multiple instance learning for image classification and auto-annotation."** Proceedings of the IEEE conference on computer vision and pattern recognition. 2015.  [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Deep+multiple+instance+learning+for+image+classification+and+auto-annotation.&btnG=) [[Paper]](https://openaccess.thecvf.com/content_cvpr_2015/html/Wu_Deep_Multiple_Instance_2015_CVPR_paper.html) ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

3. Ilse, Maximilian, Jakub Tomczak, and Max Welling. **"Attention-based deep multiple instance learning."** International conference on machine learning. PMLR, 2018. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Attention-based+deep+multiple+instance+learning&btnG=) [[Paper]](http://proceedings.mlr.press/v80/ilse18a/ilse18a.pdf) ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

4. Zhou, Bolei, et al. **"Learning deep features for discriminative localization."** Proceedings of the IEEE conference on computer vision and pattern recognition. 2016. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=learning+deep+features+for+discriminative+localization.&btnG=) [[Paper]](https://openaccess.thecvf.com/content_cvpr_2016/papers/Zhou_Learning_Deep_Features_CVPR_2016_paper.pdf)  [[Code]](http://cnnlocalization.csail.mit.edu/) ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

5. Selvaraju, Ramprasaath R., et al. **"Grad-cam: Visual explanations from deep networks via gradient-based localization."** Proceedings of the IEEE international conference on computer vision. 2017. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Grad-cam%3A+Visual+explanations+from+deep+networks+via+gradientbased+localization&btnG=) [[Paper]](http://openaccess.thecvf.com/content_ICCV_2017/papers/Selvaraju_Grad-CAM_Visual_Explanations_ICCV_2017_paper.pdf) [[Code]](https://github.com/ramprs/grad-cam/) ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

6. Chattopadhay, Aditya, et al. **"Grad-cam++: Generalized gradient-based visual explanations for deep convolutional networks."** 2018 IEEE winter conference on applications of computer vision (WACV). IEEE, 2018. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Grad-cam%2B%2B%3A+Generalized+gradient-based+visual+explanations+for+deep+convolutional+networks&btnG=) [[Paper]](https://ieeexplore.ieee.org/document/8354201?denied=) ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

7. Wang, Haofan, et al. **"Score-CAM: Score-weighted visual explanations for convolutional neural networks."** Proceedings of the IEEE/CVF conference on computer vision and pattern recognition workshops. 2020. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Score-cam%3A+Score-weighted+visual+explanations+for+convolutional+neural+networks&btnG=) [[Paper]](http://openaccess.thecvf.com/content_CVPRW_2020/papers/w1/Wang_Score-CAM_Score-Weighted_Visual_Explanations_for_Convolutional_Neural_Networks_CVPRW_2020_paper.pdf)  [[Code]](https://github.com/haofanwang/Score-CAM) ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

### 3.2 No supervision
#### 3.2.1 Self-supervised learning   
1. Caron, Mathilde, et al. **"Deep clustering for unsupervised learning of visual features."** Proceedings of the European conference on computer vision (ECCV). 2018. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Deep+clustering+for+unsupervised+learning+of+visual+features.&btnG=) [[Paper]](https://openaccess.thecvf.com/content_ECCV_2018/papers/Mathilde_Caron_Deep_Clustering_for_ECCV_2018_paper.pdf) ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)

2. Yang, Jianwei, Devi Parikh, and Dhruv Batra. **"Joint unsupervised learning of deep representations and image clusters."** Proceedings of the IEEE conference on computer vision and pattern recognition. 2016. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Joint+unsupervised+learning+of+deep+representations+and+image+clusters.&btnG=) [[Paper]](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Yang_Joint_Unsupervised_Learning_CVPR_2016_paper.pdf)  [[Code]](https://github.com/jwyang/JULE.torch) ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)

3. Xie, Junyuan, Ross Girshick, and Ali Farhadi. **"Unsupervised deep embedding for clustering analysis."** International conference on machine learning. PMLR, 2016. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Unsupervised+deep+embedding+for+clustering+analysis&btnG=) [[Paper]](http://proceedings.mlr.press/v48/xieb16.pdf) ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)

4. Noroozi, Mehdi, et al. **"Boosting self-supervised learning via knowledge transfer."** Proceedings of the IEEE conference on computer vision and pattern recognition. 2018. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Boosting+selfsupervised+learning+via+knowledge+transfer.+&btnG=) [[Paper]](https://openaccess.thecvf.com/content_cvpr_2018/papers/Noroozi_Boosting_Self-Supervised_Learning_CVPR_2018_paper.pdf) ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)

5. Tian, Yonglong, Dilip Krishnan, and Phillip Isola. **"Contrastive multiview coding."** Computer Vision–ECCV 2020: 16th European Conference, Glasgow, UK, August 23–28, 2020, Proceedings, Part XI 16. Springer International Publishing, 2020. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Contrastive+multiview+coding.&btnG=) [[Paper]](https://arxiv.org/pdf/1906.05849.pdf) [[Code]](https://github.com/HobbitLong/CMC/) ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)

6. Caron, Mathilde, et al. **"Unsupervised learning of visual features by contrasting cluster assignments."** Advances in neural information processing systems 33 (2020): 9912-9924. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Unsupervised+learning+of+visual+features+by+contrasting+cluster+assignments.+&btnG=) [[Paper]](https://proceedings.neurips.cc/paper/2020/file/70feb62b69f16e0238f741fab228fec2-Paper.pdf) [[Code]](https://github.com/facebookresearch/swav) ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)

7. Chen, Ting, et al. **"A simple framework for contrastive learning of visual representations."** International conference on machine learning. PMLR, 2020. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+simple+framework+for+contrastive+learning+of+visual+representations&btnG=) [[Paper]](http://proceedings.mlr.press/v119/chen20j/chen20j.pdf) [[Code]](https://github.com/google-research/simclr) ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)

8. Grill, Jean-Bastien, et al. "Bootstrap your own latent-a new approach to self-supervised learning." Advances in neural information processing systems 33 (2020): 21271-21284. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Bootstrap+your+own+latent-a+new+approach+to+self-supervised+learning&btnG=#d=gs_cit&t=1686511742030&u=%2Fscholar%3Fq%3Dinfo%3AUDYiz5Qo5EEJ%3Ascholar.google.com%2F%26output%3Dcite%26scirp%3D0%26hl%3Den) [[Paper]](https://proceedings.neurips.cc/paper/2020/file/f3ada80d5c4ee70142b17b8192b2958e-Paper.pdf) [[Code]](https://github.com/deepmind/deepmind-research/tree/master/byol) ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)

9. Chen, Xinlei, and Kaiming He. "Exploring simple siamese representation learning." Proceedings of the IEEE/CVF conference on computer vision and pattern recognition. 2021. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Exploring+simple+siamese+representation+learning.&btnG=) [[Paper]](https://openaccess.thecvf.com/content/CVPR2021/papers/Chen_Exploring_Simple_Siamese_Representation_Learning_CVPR_2021_paper.pdf) [[Code]](https://github.com/facebookresearch/simsiam) ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)

10. Zhuang, Chengxu, Alex Lin Zhai, and Daniel Yamins. "Local aggregation for unsupervised learning of visual embeddings." Proceedings of the IEEE/CVF International Conference on Computer Vision. 2019.
 [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=+Local+aggregation+for+unsupervised+learning+of+visual+embeddings.&btnG=) [[Paper]](https://openaccess.thecvf.com/content_ICCV_2019/papers/Zhuang_Local_Aggregation_for_Unsupervised_Learning_of_Visual_Embeddings_ICCV_2019_paper.pdf) ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)

#### 3.2.2 Unsupervised representation learning   
1. Arthur, David, and Sergei Vassilvitskii. **"K-means++ the advantages of careful seeding."** Proceedings of the eighteenth annual ACM-SIAM symposium on Discrete algorithms. 2007. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=K-means%2B%2B+the+advantages+of+careful+seeding&btnG=) [[Paper]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=K-means%2B%2B+the+advantages+of+careful+seeding&btnG=) ![](https://img.shields.io/badge/-unsupervised%20learning-red)

2. Yang, Jianwei, Devi Parikh, and Dhruv Batra. "Joint unsupervised learning of deep representations and image clusters." Proceedings of the IEEE conference on computer vision and pattern recognition. 2016. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Joint+unsupervised+learning+of+deep+representations+and+image+clusters&btnG=) [[Paper]](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Yang_Joint_Unsupervised_Learning_CVPR_2016_paper.pdf) [[Code]](https://github.com/jwyang/JULE.torch) ![](https://img.shields.io/badge/-unsupervised%20learning-red)

3. Ji, Zeguang, et al. "SEDLNet: An unsupervised precise lightweight extraction method for farmland areas." Computers and Electronics in Agriculture 210 (2023): 107886.  [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=SEDLNet%3A+An+unsupervised+precise+lightweight+extraction+method+for+farmland+areas&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169923002740)

## 4. 🤖 Applications

### 4.1 Plant health

Instructions are used in various human-computer interaction (HCI) tasks, such as virtual assistants, chatbots, etc. 

1. Coletta, Luiz FS, et al. **"Novelty detection in UAV images to identify emerging threats in eucalyptus crops."** Computers and Electronics in Agriculture 196 (2022): 106901. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Novelty+detection+in+UAV+images+to+identify+emerging+threats+in+eucalyptus+crops&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169922002186?casa_token=ZFhy1QK7aakAAAAA:wI-NrE3CAa8ph4hZ_iuU-qB0hXz6c6Kpn4f5P301ZI7qxFC4R6mxiOOogDMET4qBwo8zhARxUnE)  ![](https://img.shields.io/badge/-active--learning-brightgreen)

2. Bollis, Edson, et al. **"Weakly supervised attention-based models using activation maps for citrus mite and insect pest classification."** Computers and Electronics in Agriculture 195 (2022): 106839. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Weakly+supervised+attention-based+models+using+activation+maps+for+citrus+mite+and+insect+pest+classification&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169922001569?casa_token=ELjQTHzpJpIAAAAA:7o5dvi6KmPG3KBoC1EfUSdwb544-Gr9c2SUrhMoIJEx2OQzDMX9vhRMRpyMCk8pIJ5hPgRMu8ME)  ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

3. Monowar, Muhammad Mostafa, et al. **"Self-Supervised Clustering for Leaf Disease Identification."** Agriculture 12.6 (2022): 814. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Self-Supervised+Clustering+for+Leaf+Disease+Identification&btnG=) [[Paper]](https://www.mdpi.com/2077-0472/12/6/814)  ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)

4. Kim, Taejoo, et al. **"Instance-Aware Plant Disease Detection by Utilizing Saliency Map and Self-Supervised Pre-Training."** Agriculture 12.8 (2022): 1084. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Instance-Aware+Plant+Disease+Detection+by+Utilizing+Saliency+Map+and+Self-Supervised+Pre-Training&btnG=) [[Paper]](https://www.mdpi.com/2077-0472/12/8/1084)  ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)

5. Li, Yang, and Xuewei Chao. **"Semi-supervised few-shot learning approach for plant diseases recognition."** Plant Methods 17 (2021): 1-10. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Semi-supervised+few-shot+learning+approach+for+plant+diseases+recognition&btnG=) [[Paper]](https://link.springer.com/article/10.1186/s13007-021-00770-1)  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

6. Fang, Uno, et al. **"Self-supervised cross-iterative clustering for unlabeled plant disease images."** Neurocomputing 456 (2021): 36-48. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Self-supervised+cross-iterative+clustering+for+unlabeled+plant+disease+images&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0925231221008195?casa_token=FDyn5_5p9Z4AAAAA:5Pa6vYQxPOq2UUyI9MDEW4sze8j9jnDTyHEAJOuV0pAFjEE4FXHjAzJfioZKHdqTf5wZiCoXKC8)  ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)

7. Bollis, Edson, Helio Pedrini, and Sandra Avila. **"Weakly supervised learning guided by activation mapping applied to a novel citrus pest benchmark."** Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition Workshops. 2020. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Weakly+Supervised+Learning+Guided+by+Activation+Mapping+Applied+to+a+Novel+Citrus+Pest+Benchmark&btnG=) [[Paper]](https://openaccess.thecvf.com/content_CVPRW_2020/html/w5/Bollis_Weakly_Supervised_Learning_Guided_by_Activation_Mapping_Applied_to_a_CVPRW_2020_paper.html)  ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

8. Kim, Wan-Soo, Dae-Hyun Lee, and Yong-Joo Kim. **"Machine vision-based automatic disease symptom detection of onion downy mildew."** Computers and Electronics in Agriculture 168 (2020): 105099. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Machine+vision-based+automatic+disease+symptom+detection+of+onion+downy+mildew&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169919312384?casa_token=t87d75GPawEAAAAA:6CaaYYmbO0npqZUS_Z8vc1iSyWwleVrXE09-6EH_PFreuiouNor3j8iaJU63wXHO0l8v3aLee2s)  ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

9. Amorim, Willian Paraguassu, et al. **"Semi-supervised learning with convolutional neural networks for UAV images automatic recognition."** Computers and Electronics in Agriculture 164 (2019): 104932. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Semi-supervised+learning+with+convolutional+neural+networks+for+UAV+images+automatic+recognition&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169919305137?casa_token=qXrhLwpucfEAAAAA:8hXzr4MjJ99ilbJrmRv7YzqRz-F-xarGFbnHFiVNh-3JEMMCmFxj41VCkLhKt_21lTE0p5n6Jy4)  ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)

10. Lu, Jiang, et al. **"An in-field automatic wheat disease diagnosis system."** Computers and electronics in agriculture 142 (2017): 369-379. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=An+in-field+automatic+wheat+disease+diagnosis+system&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169917305999?casa_token=0xuJdaxkrScAAAAA:4XdlseWCH5VKNQxwuhFIN41Xi4dSOpDUXzfVbEtMMQvDrjrXee9rFsAhljK9bjIVP5ZvqZ9C9iQ)  ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

11. Wu, Yang, and Lihong Xu. **"Crop organ segmentation and disease identification based on weakly supervised deep neural network."** Agronomy 9.11 (2019): 737. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=%22Crop+Organ+Segmentation+and+Disease+Identification+Based+on+Weakly+Supervised+Deep+Neural+Network+%22&btnG=) [[Paper]](https://www.mdpi.com/2073-4395/9/11/737)  ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

12. Wang, Yinkai, et al. **"Integrated Learning-Based Pest and Disease Detection Method for Tea Leaves."** Forests 14.5 (2023): 1012. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Integrated+Learning-Based+Pest+and+Disease+Detection+Method+for+Tea+Leaves&btnG=)  [[Paper]](https://www.mdpi.com/1999-4907/14/5/1012)

13. Benfenati, Alessandro, et al. **"Unsupervised deep learning techniques for automatic detection of plant diseases: reducing the need of manual labelling of plant images."** Journal of Mathematics in Industry 13.1 (2023): 1-16. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Unsupervised+deep+learning+techniques+for+automatic+detection+of+plant+diseases%3A+reducing+the+need+of+manual+labelling+of+plant+images&btnG=)  [[Paper]](https://link.springer.com/article/10.1186/s13362-023-00133-6) ![](https://img.shields.io/badge/-unsupervised%20learning-red)

### 4.2 Weed and crop management
1. Marszalek, Michael L., et al. **"Self-supervised learning--A way to minimize time and effort for precision agriculture?."** arXiv preprint arXiv:2204.02100 (2022). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Self-supervised+learning--A+way+to+minimize+time+and+effort+for+precision+agriculture%3F&btnG=) [[Paper]](https://arxiv.org/abs/2204.02100)  ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)

2. Yang, Yana, et al. **"Dissimilarity-based active learning for embedded weed identification."** Turkish Journal of Agriculture and Forestry 46.3 (2022): 390-401. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Dissimilarity-based+active+learning+for+embedded+weed+identification&btnG=) [[Paper]](https://journals.tubitak.gov.tr/agriculture/vol46/iss3/11/) ![](https://img.shields.io/badge/-active--learning-brightgreen)

3. Nong, Chunshi, Xijian Fan, and Junling Wang. **"Semi-supervised Learning for Weed and Crop Segmentation Using UAV Imagery."** Frontiers in Plant Science 13 (2022). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Semi-supervised+Learning+for+Weed+and+Crop+Segmentation+Using+UAV+Imagery&btnG=) [[Paper]](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9283949/)  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

4. Güldenring, Ronja, and Lazaros Nalpantidis. **"Self-supervised contrastive learning on agricultural images."** Computers and Electronics in Agriculture 191 (2021): 106510. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Self-supervised+contrastive+learning+on+agricultural+images&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169921005275)  ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)

5. Shorewala, Shantam, et al. **"Weed density and distribution estimation for precision agriculture using semi-supervised learning."** IEEE access 9 (2021): 27971-27986. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Weed+Density+and+Distribution+Estimation+for+Precision+Agriculture+Using+Semi-Supervised+Learning&btnG=) [[Paper]](https://ieeexplore.ieee.org/abstract/document/9350244)  ![](https://img.shields.io/badge/-unsupervised%20learning-red)

6. Hu, Chengsong, J. Alex Thomasson, and Muthukumar V. Bagavathiannan. **"A powerful image synthesis and semi-supervised learning pipeline for site-specific weed detection."** Computers and Electronics in Agriculture 190 (2021): 106423. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+powerful+image+synthesis+and+semi-supervised+learning+pipeline+for+site-specific+weed+detection&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169921004403?casa_token=qbLLY8XNSGoAAAAA:Xo4rcwElVN_SDaVDNPJLekHBVcgRx9tb7TMKXFsfmKT_Az3LXq9ewaCHCx2MMhDl0MDBNJYnH5A)  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

7. dos Santos Ferreira, Alessandro, et al. **"Unsupervised deep learning and semi-automatic data labeling in weed discrimination."** Computers and Electronics in Agriculture 165 (2019): 104963. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Unsupervised+deep+learning+and+semi-automatic+data+labeling+in+weed+discrimination&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169919313237?casa_token=sLtTIEsj7L8AAAAA:F_01KTJcFtECjvpazMTf9MEJgDCOSWy_2ACUwV1b8XgZ9FEnE9Tz8zDNPgNRP3wd8j6jyN_Y7EU)  ![](https://img.shields.io/badge/-unsupervised%20learning-red)

8. Bah, M. Dian, Adel Hafiane, and Raphael Canals. **"Deep learning with unsupervised data labeling for weed detection in line crops in UAV images."** Remote sensing 10.11 (2018): 1690. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Deep+Learning+with+Unsupervised+Data+Labeling+for+Weed+Detection+in+Line+Crops+in+UAV+Images&btnG=) [[Paper]](https://www.mdpi.com/2072-4292/10/11/1690)  ![](https://img.shields.io/badge/-unsupervised%20learning-red)

9. Pérez-Ortiz, Maria, et al. **"A semi-supervised system for weed mapping in sunflower crops using unmanned aerial vehicles and a crop row detection method."** Applied Soft Computing 37 (2015): 533-544. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+semi-supervised+system+for+weed+mapping+in+sunflower+crops+using+unmanned+aerial+vehicles+and+a+crop+row+detection+method&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S1568494615005281?casa_token=Kx34E34LQjUAAAAA:MzVxJgy_iDyIVXTrpkUPy6amDT2IDNiDimhakt0gc8CObSyUb1fpvEZkrz5eZP-EAoUiCtbaLrE)  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

### 4.3 Fruit detection
1. Ciarfuglia, Thomas A., et al. **"Weakly and semi-supervised detection, segmentation and tracking of table grapes with limited and noisy data."** Computers and Electronics in Agriculture 205 (2023): 107624. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Weakly+and+Semi-Supervised+Detection%2C+Segmentation+and+Tracking+of+Table+Grapes+with+Limited+and+Noisy+Data&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169923000121)  ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

2. Bhattarai, Uddhav, and Manoj Karkee. **"A weakly-supervised approach for flower/fruit counting in apple orchards."** Computers in Industry 138 (2022): 103635. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+weakly-supervised+approach+for+flower%2Ffruit+counting+in+apple+orchards&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0166361522000306?casa_token=xWeCzyeEZZUAAAAA:LUjMhynGwwsck4eA-rHwfmSlEPYmSr8BRLwiSdyYLfCRMzt-jS6akIiGCRBnNR7ccLM8pcKeVLQ)  ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

3. Bellocchio, Enrico, et al. **"A novel vision-based weakly supervised framework for autonomous yield estimation in agricultural applications."** Engineering Applications of Artificial Intelligence 109 (2022): 104615. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+novel+vision-based+weakly+supervised+framework+for+autonomous+yield+estimation+in+agricultural+applications&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0952197621004310?casa_token=-9FqEhV_TIwAAAAA:FsWlWxH_tdGfZ-R2BoinYcHee6s-vxMjNIu-yPkv-qE7C6DGpXN4qA-s_o-tNPNvJwA2rX_Dk7U)  ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

4. Casado-García, A., et al. **"Semi-supervised deep learning and low-cost cameras for the semantic segmentation of natural images in viticulture."** Precision Agriculture (2022): 1-26. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Semi-supervised+deep+learning+and+low-cost+cameras+for+the+semantic+segmentation+of+natural+images+in+viticulture&btnG=) [[Paper]](https://link.springer.com/article/10.1007/s11119-022-09929-9)  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

5. Khaki, Saeed, et al. **"Deepcorn: A semi-supervised deep learning method for high-throughput image-based corn kernel counting and yield estimation."** Knowledge-Based Systems 218 (2021): 106874. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=DeepCorn%3A+A+semi-supervised+deep+learning+method+for+high-throughput+image-based+corn+kernel+counting+and+yield+estimation&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0950705121001374?casa_token=l6_EWtXTZKYAAAAA:-66kxmrbl64ho7xiOI12o2fopzjHy83TQznz_hYZDktYp13qRlEysM2kepX2eUVaiiI0FlJheuU)  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

6. Bellocchio, Enrico, et al. **"Combining domain adaptation and spatial consistency for unseen fruits counting: a quasi-unsupervised approach."** IEEE Robotics and Automation Letters 5.2 (2020): 1079-1086. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Combining+domain+adaptation+and+spatial+consistency+for+unseen+fruits+counting%3A+A+quasi+unsupervised+approach&btnG=) [[Paper]](https://ieeexplore.ieee.org/abstract/document/8957569?casa_token=KMOqwa2X0x8AAAAA:Wnywsh46mUKKU8D_8U_HY3JLODoA2MYFGzGqA7k3MLGXNVXKSR4Nh8kaXjj9LHNEe3GHpU2zsiw)  ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

7. Bellocchio, Enrico, et al. **"Weakly supervised fruit counting for yield estimation using spatial consistency."** IEEE Robotics and Automation Letters 4.3 (2019): 2348-2355. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Weakly+Supervised+Fruit+Counting+for+Yield+Estimation+Using+Spatial+Consistency&btnG=) [[Paper]](https://ieeexplore.ieee.org/abstract/document/8661632?casa_token=JCFKLG19GCwAAAAA:TRJtK24bhVT51_jKh3pODODsooRuiimzF_6uKq7LbgmuyFtVkKv_q7gAsoTKcdfTdgGyfMTSQ5M) ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

8. Roy, Pravakar, et al. **"Vision-based preharvest yield mapping for apple orchards."** Computers and Electronics in Agriculture 164 (2019): 104897. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Vision-based+preharvest+yield+mapping+for+apple+orchards&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169919303436?casa_token=0cpG4d1hc50AAAAA:LysqbihEr3zY5-2Ub7zl878HhgwHCQgzOt5wysTou9B1bKXdXxxkkcr2rZBVXgfku30onUkaCZE)  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

### 4.4 Aquaculture
1. Kong, Qingchen, et al. **"A recurrent network based on active learning for the assessment of fish feeding status."** Computers and Electronics in Agriculture 198 (2022): 106979. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+recurrent+network+based+on+active+learning+for+the+assessment+of+fish+feeding+status&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169922002964?casa_token=3sEdz3v21LgAAAAA:Xt0sn8l-FcWHyTSPuTPg-zR1nIkH59hhu0yl2uju8z2kDi2yjGVYfIo-egNbffOruatbiO4C6Qw)  ![](https://img.shields.io/badge/-active--learning-brightgreen)

### 4.5 Plant Phenotyping
1. Lin, Xufeng, et al. **"Self-Supervised Leaf Segmentation under Complex Lighting Conditions."** Pattern Recognition 135 (2023): 109021. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Self-Supervised+Leaf+Segmentation+under+Complex+Lighting+Conditions&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0031320322005015?casa_token=hbczlttXx3QAAAAA:Sj_D4jBQEBfVQpM2H1V3KTVqvFyzz1rvErGPqMFFIdVWSqiJMJMYONoWnRHGONStKrc4p-Vt0oM)  [[Code]](https://github.com/lxfhfut/Self-Supervised-Leaf-Segmentation) ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

2. Tschand, Arya. **"Semi-supervised machine learning analysis of crop color for autonomous irrigation."** Smart Agricultural Technology 3 (2023): 100116. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Semi-Supervised+Machine+Learning+Analysis+of+Crop+Color+for+Autonomous+Irrigation&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S2772375522000818) ![](https://img.shields.io/badge/-unsupervised%20learning-red)

3. Blok, Pieter M., et al. **"Active learning with MaskAL reduces annotation effort for training Mask R-CNN on a broccoli dataset with visually similar classes."** Computers and Electronics in Agriculture 197 (2022): 106917. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Active+learning+with+MaskAL+reduces+annotation+effort+for+training+Mask+R-CNN+on+a+broccoli+dataset+with+visually+similar+classes&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169922002344) [[Code]](https://github.com/pieterblok/maskal) ![](https://img.shields.io/badge/-active--learning-brightgreen)

4. Rawat, Shivangana, et al. **"How Useful Is Image-Based Active Learning for Plant Organ Segmentation?."** Plant Phenomics 2022 (2022). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=How+Useful+Is+Image-Based+Active+Learning+for+Plant+Organ+Segmentation%3F&btnG=) [[Paper]](https://downloads.spj.sciencemag.org/plantphenomics/2022/9795275.pdf)   ![](https://img.shields.io/badge/-active--learning-brightgreen)

5. Li, Lei, et al. **"Leaf vein segmentation with self-supervision."** Computers and Electronics in Agriculture 203 (2022): 107352. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Leaf+vein+segmentation+with+self-supervision&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169922006603?casa_token=DgMIEFP-89YAAAAA:8nAwxkwH7QDAPJutUAtUdWe0vmWvwB2apcT1huH4tRQLAQF1ml2B_2h0mIrHOujVsLoiSTJsZi0)  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

6. Zhang, Xin, et al. **"The Self-Supervised Spectral–Spatial Vision Transformer Network for Accurate Prediction of Wheat Nitrogen Status from UAV Imagery."** Remote Sensing 14.6 (2022): 1400. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=The+Self-Supervised+Spectral%E2%80%93Spatial+Vision+Transformer+Network+for+Accurate+Prediction+of+Wheat+Nitrogen+Status+from+UAV+Imagery&btnG=) [[Paper]](https://www.mdpi.com/2072-4292/14/6/1400)  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

7. Qiang, Zhuang, Jingmin Shi, and Fanhuai Shi. **"Phenotype Tracking of Leafy Greens Based on Weakly Supervised Instance Segmentation and Data Association."** Agronomy 12.7 (2022): 1567. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Phenotype+Tracking+of+Leafy+Greens+Based+on+Weakly+Supervised+Instance+Segmentation+and+Data+Association&btnG=) [[Paper]](https://www.mdpi.com/2073-4395/12/7/1567)  ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

8. Adke, Shrinidhi, et al. **"Supervised and weakly supervised deep learning for segmentation and counting of cotton bolls using proximal imagery."** Sensors 22.10 (2022): 3688. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Supervised+and+Weakly+Supervised+Deep+Learning+for+Segmentation+and+Counting+of+Cotton+Bolls+Using+Proximal+Imagery&btnG=) [[Paper]](https://www.mdpi.com/1424-8220/22/10/3688)  ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

9. Dandrifosse, Sébastien, et al. **"Deep learning for wheat ear segmentation and ear density measurement: From heading to maturity."** Computers and Electronics in Agriculture 199 (2022): 107161. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Deep+learning+for+wheat+ear+segmentation+and+ear+density+measurement%3A+From+heading+to+maturity&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169922004781?casa_token=t3uK4RCbltYAAAAA:9p9kRe3Hzm0VOlGPIb7x5T2mAB9SBFkLfXxQUYi0T-Nsbs2lQlii43OYWtowG55tT8VCQUUdeMw)  ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

10. Petti, Daniel, and Changying Li. **"Weakly-supervised learning to automatically count cotton flowers from aerial imagery."** Computers and Electronics in Agriculture 194 (2022): 106734.  [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Weakly-supervised+learning+to+automatically+count+cotton+flowers+from+aerial+imagery&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169922000515?casa_token=X9YWbhowQK4AAAAA:1vrbgGZ8p8NA8cUoTnNtg4FCv9B9e_8NXqkxcCiQX0Xf-sl8bHA_p7dgHQjsN56YcSennvOjzHs)  ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

11. Kim, Wan-Soo, et al. **"Weakly supervised crop area segmentation for an autonomous combine harvester."** Sensors 21.14 (2021): 4801. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Weakly+Supervised+Crop+Area+Segmentation+for+an+Autonomous+Combine+Harvester&btnG=) [[Paper]](https://www.mdpi.com/1424-8220/21/14/4801)  ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

12. Siddique, Abubakar, Amy Tabb, and Henry Medeiros. **"Self-supervised Learning for Panoptic Segmentation of Multiple Fruit Flower Species."** IEEE Robotics and Automation Letters 7.4 (2022): 12387-12394. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Self-supervised+Learning+for+Panoptic+Segmentation+of+Multiple+Fruit+Flower+Species&btnG=) [[Paper]](https://ieeexplore.ieee.org/document/9928359?casa_token=UptjC3JQnB4AAAAA:ktJySPWen4i5GCfi_DfXvDTW61vG_lrRs6jEz5Pg8KBDMTEYpNZBNa_2OObIBa8JShJymAwnQu0)  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

13. Najafian, Keyhan, et al. **"A semi-self-supervised learning approach for wheat head detection using extremely small number of labeled samples."** Proceedings of the IEEE/CVF International Conference on Computer Vision. 2021. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+Semi-self-supervised+Learning+Approach+for+Wheat+Head+Detection+using+Extremely+Small+Number+of+Labeled+Samples&btnG=) [[Paper]](https://openaccess.thecvf.com/content/ICCV2021W/CVPPA/html/Najafian_A_Semi-Self-Supervised_Learning_Approach_for_Wheat_Head_Detection_Using_Extremely_ICCVW_2021_paper.html)  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

14. Fourati, Fares, Wided Souidene Mseddi, and Rabah Attia. **"Wheat head detection using deep, semi-supervised and ensemble learning."** Canadian Journal of Remote Sensing 47.2 (2021): 198-208. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=An+original+framework+for+Wheat+Head+Detection+using+Deep%2C+Semi-supervised+and+Ensemble+Learning+within+Global+Wheat+Head+Detection+%28GWHD%29+Dataset&btnG=) [[Paper]](https://www.tandfonline.com/doi/abs/10.1080/07038992.2021.1906213)  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

15. Ghosal, Sambuddha, et al. **"A weakly supervised deep learning framework for sorghum head detection and counting."** Plant Phenomics (2019). [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=A+Weakly+Supervised+Deep+Learning+Framework+for+Sorghum+Head+Detection+and+Counting&btnG=) [[Paper]](https://spj.science.org/doi/full/10.34133/2019/1525874)  ![](https://img.shields.io/badge/-semi--supervised%20learning-yellow)

16. Chandra, Akshay L., et al. **"Active learning with point supervision for cost-effective panicle detection in cereal crops."** Plant Methods 16 (2020): 1-16. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Active+learning+with+point+supervision+for+cost-effective+panicle+detection+in+cereal+crops&btnG=) [[Paper]](https://link.springer.com/article/10.1186/s13007-020-00575-8)  ![](https://img.shields.io/badge/-active--learning-brightgreen)

17. Ayalew, Tewodros W., Jordan R. Ubbens, and Ian Stavness. **"Unsupervised domain adaptation for plant organ counting."** Computer Vision–ECCV 2020 Workshops: Glasgow, UK, August 23–28, 2020, Proceedings, Part VI 16. Springer International Publishing, 2020. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Unsupervised+Domain+Adaptation+For+Plant+Organ+Counting&btnG=) [[Paper]](https://link.springer.com/chapter/10.1007/978-3-030-65414-6_23) ![](https://img.shields.io/badge/-unsupervised%20learning-red)

18. Valerio Giuffrida, Mario, et al. **"Leaf counting without annotations using adversarial unsupervised domain adaptation."** Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition Workshops. 2019. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=%22Leaf+counting+without+annotations+using+adversarial+unsupervised+domain+adaptation%22&btnG=) [[Paper]](https://openaccess.thecvf.com/content_CVPRW_2019/html/CVPPP/Giuffrida_Leaf_Counting_Without_Annotations_Using_Adversarial_Unsupervised_Domain_Adaptation_CVPRW_2019_paper.html) ![](https://img.shields.io/badge/-unsupervised%20learning-red)

19. Wang, Yi, and Lihong Xu. **"Unsupervised segmentation of greenhouse plant images based on modified Latent Dirichlet Allocation."** PeerJ 6 (2018): e5036. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=%22Unsupervised+segmentation+of+greenhouse+plant+images+based+on+modified+latent+dirichlet+allocation%22&btnG=) [[Paper]](https://peerj.com/articles/5036/) ![](https://img.shields.io/badge/-unsupervised%20learning-red)

20. Zhang, Ping, and Lihong Xu. **"Unsupervised segmentation of greenhouse plant images based on statistical method."** Scientific reports 8.1 (2018): 1-13. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Unsupervised+segmentation+of+greenhouse+plant+images+based+on+statistical+method&btnG=) [[Paper]](https://link.springer.com/content/pdf/10.1038/s41598-018-22568-3.pdf) ![](https://img.shields.io/badge/-unsupervised%20learning-red)


### 4.6 Postharvest quality assessment
1. Liu, Yisen, et al. **"Joint optimization of autoencoder and self-supervised classifier: anomaly detection of strawberries using hyperspectral imaging."** Computers and Electronics in Agriculture 198 (2022): 107007. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Joint+optimization+of+autoencoder+and+Self-Supervised+Classifier%3A+Anomaly+detection+of+strawberries+using+hyperspectral+imaging&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0168169922003246?casa_token=mbiSlzaiRvEAAAAA:6rfTcrs7MG1etkv2cGSz75ZfjBAUc0OdCa5l32TvDYmXNrqJ2iRcbNjC4Ee-F-rq4L0bLx3gz_4)  ![](https://img.shields.io/badge/-self--supervised%20leaning-blue)

2. Li, Weitao, et al. **"Greengage grading using stochastic configuration networks and a semi-supervised feedback mechanism."** Information Sciences 488 (2019): 1-12. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Greengage+grading+using+stochastic+configuration+networks+and+a+semi-supervised+feedback+mechanism&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0020025519301501?casa_token=n_LudCJnoLQAAAAA:8OxTDeg7i8axhkrkSPksjPHqHKj_ecmbVXDEFqQaipZJ7z8FAOeptHb03E-Wzw2KUCvvjZwjz4M)  ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)

3. Marino, Sofia, Pierre Beauseroy, and André Smolarz. **"Weakly-supervised learning approach for potato defects segmentation."** Engineering Applications of Artificial Intelligence 85 (2019): 337-346. [[Google Scholar]](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C23&q=Weakly-supervised+learning+approach+for+potato+defects+segmentation&btnG=) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0952197619301630?casa_token=M83Hltqn6dkAAAAA:T-gCy-NLjAKyuIeu-b2ccq_b9xYK9UTKkg1VOgF49C_1mz51bI5YIkThmkb6Hnly7Q4KUjW-aXU)  ![](https://img.shields.io/badge/-weakly%20supervised%20leaning-orange)



<!-- TODO: tweets & slides? -->

---

<!-- omit in toc -->
## ⭐ Star History

[![Star History Chart](https://api.star-history.com/svg?repos=DongChen06/Label-efficient-in-Agriculture&type=Date)](https://star-history.com/#DongChen06/Label-efficient-in-Agriculture&Date)
