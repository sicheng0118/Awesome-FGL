# Notes on [ 2021 arXiv ] Position Paper on FGL

⭐【基本信息】

![](/Attachments/2021-arXiv-Position_Paper_on_FGL/Info.png)

---

⭐【速读】

![](/Attachments/2021-arXiv-Position_Paper_on_FGL/KeyPoint.png)

***<p align="center">探讨FGL的定义、分类、应用和挑战</p>*** 

---

⭐【摘要】

- Background
  - In some **privacy-sensitive scenarios** (like finance, and healthcare), **training a GNN model CENTRALLY** faces challenges due to the **distributed data silos**.
  - Federated Learning is an emerging technique that can **collaboratively train a shared model while keeping the data decentralized**.
- Contributions
  - Considering **how graph data are distributed among clients**, we propose four types of FGL: **inter-graph FL**, intra-graph FL, and **graph-structure FL**, where intra-graph FL is further divided into **horizontal and vertical FGL**.
 
---

⭐【一句话总结】

这篇论文探讨的问题是**在涉及分散存储且隐私敏感的数据时，如何通过联邦学习（Federated Learning，FL）实现图神经网络（Graph Neural Networks，GNN）的分布式训练**，并将联邦图学习（Federated Graph Learning，FGL）总结为 4 类：**图间FL、水平图内FL、垂直图内FL和图结构FL**，介绍了每种类型的特点、应用场景以及面临的主要挑战，如非独立同分布（Non-IID）图结构、数据孤岛、实体匹配和安全数据共享等，同时指出了未来研究的方向。

**Q1: 本文的动机/试图解决的问题是什么？**

A: 本文认为**集中式训练GNN模型的传统方法，在处理分散存储且隐私敏感的数据时存在Failure Case，而GNN+FL是应对该场景的一类可行方案**。随着FGL越来越受关注，一篇概述其**定义、技术细节、所面临的挑战和潜在解决方案**的文章就有了必要。

**要点如下：**
1. FGL的分类：依据 **“How graph data are distributed among clients”** 的划分标准，将
2. FGL在实际应用中可能遇到的挑战：

**Q2: 在该问题上有哪些相关研究？**

A：

别人的研究有何不足

方法/如何解决

**Q3: 本文的创新点/如何解决这个问题？**

A：提出了什么样的分类标准，具体类别有哪些

论文做了哪些实验/所提方法的优势是什么

**Q4: 有什么可以进一步探索的点？**

A：
