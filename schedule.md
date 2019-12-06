---
title: 'NeurIPS 2019 Optimization Foundations for Reinforcement Learning Workshop'
layout: default
---

# Schedule

| Time    | Event |
| ------- | -------- |
| 08:00 - 08:10 | **Opening Remarks** |
| 08:10 - 08:50 | **Invited Talk** - [Mengdi Wang][mengdi]: *TBA*|
| 08:50 - 09:10 | **Contributed Talk** - Lior Shani, Yonathan Efroni, Shie Mannor: <a href="assets/accepted_papers/2.pdf">*Adaptive Trust Region Policy Optimization: Convergence and Faster Rates of regularized MDPs*</a> |
| 09:10 - 09:30 | **Spotlight** |
| | - David Brandfonbrener, Joan Bruna: <a href="assets/accepted_papers/7.pdf">*Geometric Insights into the Convergence of Nonlinear TD Learning*</a>|
| | - Tom Zahavy, Haim Kaplan, Alon Cohen, Yishay Mansour: <a href="assets/accepted_papers/10.pdf">*Apprenticeship Learning via Frank-Wolfe*</a>|	
| | - Nikos Karampatziakis, John Langford, Paul Mineiro: <a href="assets/accepted_papers/22.pdf">*Empirical Likelihood for Contextual Bandits*</a>|
| | - Ofir Nachum, Bo Dai, Ilya  Kostrikov, Dale  Schuurmans: <a href="assets/accepted_papers/44.pdf">*ALGAE: Policy Gradient from Arbitrary Experience*</a>	|
| 09:30 - 10:30 | **Poster and Coffee Break** |
| 10:30 - 11:10 | **Invited Talk** - [Sham Kakade][sham]: *The Provable Effectiveness of Policy Gradient Methods in Reinforcement Learning*|
||Reinforcement learning is now the dominant paradigm for how an agent learns to interact with the world in order to achieve some long term objectives. Here, policy gradient methods are among the most effective methods in challenging reinforcement learning problems, due to that they: are applicable to any differentiable policy parameterization; admit easy extensions to function approximation; easily incorporate structured state and action spaces; are easy to implement in a simulation based, model-free manner.

However, little is known about even their most basic theoretical convergence properties, including:
 - do they converge to a globally optimal solution, say with a sufficiently rich policy class?
 - how well do they cope with approximation error, say due to using a class of neural policies?
 - what is their finite sample complexity?
This talk will survey a number of results on these basic questions. We will  highlight the interplay of theory, algorithm design, and practice.

Joint work with: Alekh Agarwal, Jason Lee, Gaurav Mahajan|
| 11:10 - 11:40 | **Panel Discussion** - [Richard Sutton][rich] and [Doina Precup][doina] |
| 11:40 - 12:20 | **Spotlight** |
| | - Donghwan Lee, Niao He： <a href="assets/accepted_papers/27.pdf">*Analysis of Q-Learning: Switching System Approach*</a>|
| | - Aaron Sidford, Mengdi Wang, Lin Yang, Yinyu Ye: <a href="assets/accepted_papers/33.pdf">*Solving Discounted Stochastic Two-Player Games with Near-Optimal Time and Sample Complexity*</a>|
| | - Zuyue Fu, Zhuoran Yang, Yongxin Chen, Zhaoran Wang: <a href="assets/accepted_papers/42.pdf">*Actor-Critic Provably Finds Nash Equilibria of Linear-Quadratic Mean-Field Games*</a>|
| | - Ziyang Tang, Yihao Feng, Lihong Li, Denny Zhou, Qiang Liu: <a href="assets/accepted_papers/48.pdf">*Harnessing Infinite-Horizon Off-Policy Evaluation: Double Robustness via Duality*</a>|
| | - Rodrigo A Toro Icarte, Ethan Waldie, Toryn  Klassen,  Richard Valenzano, Margarita  Castro, Sheila A.  McIlraith: <a href="assets/accepted_papers/49.pdf">*Learning Reward Machines for Partially Observable Reinforcement Learning*</a>|	
| | - Simon Du, Sham Kakade, Ruosong Wang, Lin Yang: <a href="assets/accepted_papers/53.pdf">*Is a Good Representation Sufficient for Sample Efficient Reinforcement Learning?*</a>|
| | - Minshuo Chen, Yizhou Wang, Tianyi  Liu, Xingguo Li, Zhuoran Yang, Zhaoran Wang, Tuo Zhao: <a href="assets/accepted_papers/54.pdf">*On Computation and Generalization of Generative Adversarial Imitation Learning*</a>|
| | - Philip Amortila, Doina Precup, Prakash  Panangaden, Marc G. Bellemare: <a href="assets/accepted_papers/69.pdf">*A Distributional Analysis of Sampling-Based Reinforcement Learning Algorithms*</a>|
| 12:20 - 14:00 | **Lunch** |
| 14:00 - 14:40 | **Invited Talk** - [Benjamin Van Roy][ben]: *Reinforcement Learning Beyond Optimization*|
| 14:40 - 15:20 | **Invited Talk** - [Shipra Agrawal][shipra]: *Learning in structured MDPs with convex cost function: improved regret bounds for inventory management*|
||We present a learning algorithm for the stochastic inventory control problem under lost sales penalty and positive lead times, when the demand distribution is a priori unknown. Our main result is a regret bound of $$O(L\sqrt{T}+D)$$ for the algorithm, where T is the time horizon, L is the fixed and known lead time, and D is an unknown parameter of the demand distribution described roughly as the number of time steps needed to generate enough demand for depleting one unit of inventory. Our results significantly improve the existing regret bounds for this problem. Notably, even though the state space of the underlying Markov Decision Process (MDP) in this problem is continuous and L-dimensional, our regret bounds depend linearly on L. Our techniques utilize convexity of the long run average cost  and a newly derived bound on the `bias' of base-stock policies, to establish an almost blackbox  connection between the problem of learning and optimization in such MDPs and stochastic convex bandit optimization. The techniques presented here may be of independent interest for other settings that involve learning large structured MDPs but with convex cost functions.|
| 15:20 - 16:20 | **Poster and Coffee Break** |
| 16:20 - 17:00 | **Invited Talk** - [Huizhen Yu][huizhen]: *On the Convergence of GTD($$\lambda$$) with General $$\lambda$$* |
||Gradient temporal-difference (GTD) algorithms are an important family of extensions of the standard TD algorithm, overcoming the stability issues in off-policy learning with function approximation by minimizing the projected Bellman error using stochastic gradient descent (SGD). In this talk, we consider GTD($\lambda$) for policy evaluation in the case of linear function approximation and finite-space Markov decision processes (MDPs) with discounted rewards. GTD($\lambda$) differs from the typical SGD algorithm for minimizing an objective function, in the following way. In an MDP, each stationary policy is associated with a family of Bellman equations. By selecting the values of the eligibility trace parameters, $\lambda$, we determine the Bellman operator that defines the objective function. This choice influences both the approximation error and learning behavior of the resulting algorithm. We first describe a dynamic scheme to judiciously set $\lambda$ in a history-dependent way. This scheme is based on the idea of randomized stopping times and generalized Bellman equations, and it is useful for balancing the bias-variance tradeoff in off-policy learning. We then present asymptotic convergence results for several variations of GTD($\lambda$), including saddle-point and mirror-descent TD variants, for different choices of $\lambda$: constant, state-dependent, and history-dependent. These convergence results are obtained by combining special properties of the joint state and eligibility trace process in TD learning with ergodic theory for weak Feller Markov chains, mean-ODE-based proof methods, and convex optimization theory. Our results not only resolve long-standing open questions regarding the convergence of GTD($\lambda$) but also provide the basis for using a broader class of generalized Bellman operators for approximate policy evaluation with linear TD methods.|
| 17:00 - 17:20 | **Contributed Talk**- Jonathan Lee, Ching-An Cheng, Ken Goldberg, Byron Boot: <a href="assets/accepted_papers/55.pdf">*Continuous Online Learning and New Insights to Online Imitation Learning*</a> |
| 17:20 - 17:40 | **Contributed Talk** - Naman Agarwal, Elad Hazan, Karan Singh:  <a href="assets/accepted_papers/37.pdf">*Logarithmic Regret for Online Control*</a>|
| 17:40 - 18:00 | **Closing Remarks** |

<!-- [speakers]: #speakers -->
[sham]: https://homes.cs.washington.edu/~sham/
[shipra]: http://www.columbia.edu/~sa3305/
[ben]: https://web.stanford.edu/~bvr/
[mengdi]: https://mwang.princeton.edu/
[huizhen]: https://directory.ualberta.ca/person/huizhen
[rich]: http://incompleteideas.net/
[doina]: https://www.cs.mcgill.ca/~dprecup/

