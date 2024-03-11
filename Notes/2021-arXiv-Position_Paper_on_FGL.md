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
  - Federated Learning can **collaboratively train a shared model while keeping the data decentralized**.
- Contributions
  - Considering **how graph data are distributed among clients**, we propose four types of FGL: **inter-graph FL**, intra-graph FL, and **graph-structure FL**, where intra-graph FL is further divided into **horizontal and vertical FGL**.
 
---

⭐【一句话总结】

这篇论文探讨的问题是**在涉及分散存储且隐私敏感的数据时，如何通过联邦学习（Federated Learning，FL）实现图神经网络（Graph Neural Networks，GNN）的分布式训练**，文中将联邦图学习（Federated Graph Learning，FGL）总结为 4 类：**图间FL、水平图内FL、垂直图内FL和图结构FL**，介绍了每一类的特点、应用场景以及面临的主要挑战，如非独立同分布（Non-IID）图结构、数据孤岛、实体匹配和安全数据共享等。

**Q1: 本文的动机/试图解决的问题是什么？**

A: 本文认为**集中式训练GNN模型的传统方法，在处理分散存储且隐私敏感的数据时存在Failure Case，而GNN+FL是应对该场景的一类可行方案**。随着FGL越来越受关注，一篇概述其**定义、技术细节、潜在挑战和可能的解决方案**的文章就有了必要。

**要点如下：**
1. FGL的分类：依据 **“How graph data are distributed among clients”**，将FGL划分为 4 类：inter-graph FL、intra-graph FL（包括horizontal FGL和vertical FGL）以及graph-structure FL，并展开介绍。
2. FGL在实际应用中可能遇到的挑战：非独立同分布数据（普遍存在）、Isolation of the latent entire graph（horizontal FGL）、Entities matching and secure data sharing（vertical FGL）、可用数据集（intra-graph FL）、Communication and memory consumption

**Q2: 在该问题上有哪些相关研究？**

A：已经有相关研究将FL引入GNN来应对multi-user场景，但目前一份阐明FGL定义与挑战（**尤其是足够具体的类别划分**）的文章仍悬而未决。

**相关研究如下：**
1. FGL综述：FedGraphNN（LCLR, 2021）给出了关于FGL的相对完整的Benchmark。
2. 挑战与现有研究、及其局限

**Q3: 本文提出了什么方法/如何解决这个问题？**

A：本文基于 “How graph data are distributed” 的角度为FGL分类，讨论了每一类的定义与应用，分析了每一类的潜在挑战和可能的解决方案。

**具体内容如下：** 

1. inter-graph FL：Each sample of clients is of **graph data**, and global model performs **graph-level tasks**. The most typical application is to learn the structure of
molecules or the properities of drug. 
   
<div align=center>
<img src="/Attachments/2021-arXiv-Position_Paper_on_FGL/kp1.png">
</div>

2. horizontal FGL

3. vertical FGL

4. graph-structure FGL：不仅数据以图的形式呈现，client之间存在的图拓扑关系，也作为模型的一部分（在其它的FGL中，client之间的拓扑结构更像是同一个集合中的元素关系？）

**Q4: 有什么可以进一步探索的点？**

A：
