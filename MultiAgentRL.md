# 多智能体强化学习算法笔记
## QMIX: Monotonic Value Function Factorisation for Deep Multi-Agent Reinforcement Learning

Personaly favorite work. Based on the value decomposition network(VDN), it proposes the monotonic function to fit the relationship between the $Q^{\mathrm{tot}}$ and $\tilde{Q}_{i}$, where $Q^{\mathrm{tot}}$ denotes the global Q value and it is calculated based on the global state and the global action. 
$\tilde{Q}_{i}$ denotes the corresponding local Q value of agent $i$, which is calculated based on the local state $s_i$ and local action $u_i$. 
Due to the monotonic property, the maximization of $Q^{\mathrm{tot}}$ equals the maximization of $\tilde{Q}_{i},\;\forall i \in \mathcal{A}$, this is also defined as Individual-Global Maximization(IGM) in QTran.

- Pros: Main idea is straight, compared with the VDN, it extends the relationship to a monotonic function, where VDN proposes an linear struction. For most cooperative scenario, QMIX can achieve better performance.
- Cons: Monotonic function is not always work for all coopearative scenario. The presenting space is limited to positive weight.

## Value-Decomposition Networks For Cooperative Multi-Agent Learning
First work in value decomposition technique. Main idea is easy, authors consider the $Q^{\mathrm{tot}}$ is a linear combination of $\tilde{Q}_{i}$. IGM is also hold ture for VDN.

## QTRAN: Learning to Factorize with Transformation for Cooperative Multi-Agent Reinforcement learning


## COMA: Counterfactual Multi-Agent Policy Gradients
This work is an art.

## COMIX: Deep Multi-Agent Reinforcement Learning for Decentralized Continuous Cooperative Control
