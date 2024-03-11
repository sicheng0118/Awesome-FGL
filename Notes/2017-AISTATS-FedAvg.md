# Notes on [ 2017 AISTATS ] FedAvg

⭐【基本信息】

<div align=center>
<img src="/Attachments/2017-AISTATS-FedAvg/Info.png">
</div>

---

⭐【速读】

<div align=center>
<img src="/Attachments/2017-AISTATS-FedAvg/KeyPoint.png" width="50%">
</div>

***<p align="center">FedAvg算法流程</p>*** 

---

⭐【摘要】

- Background
  - The performance of the model heavily relies on **a wealth of training data**. However, those data is often **privacy-sensitive, large in quantity**, or both, which **precludes logging into the data center and training the model using conventional approaches**.
  
- Contributions
  - We propose to **leave the training data distributed**, and **learn a shared model by aggregating locally-computed updates**.

