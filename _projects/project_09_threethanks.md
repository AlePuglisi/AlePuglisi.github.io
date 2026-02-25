---
title: "Centralized, Decentralized and Distributed Control of a Three-Tanks System"
excerpt: "<img align='left' src='/images/projects/ProjectThreeTanks.png' width='450' style='margin-right: 15px; margin-bottom: 15px;'/>**University Project-Completed** <br>
Networked Control Final Assignment - 2023 <br>
MATLAB - YALMIP - Simulation <br>
Modeled a benchmark control problem of a three tanks system in MATLAB, and analyzed its stability in 
continuous and discrete time. Tuned different control structures (centralized, decentralized, discontinuous)
through Linear Matrix Inequality (LMI) theory and YALMIP optimization toolbox. "
collection: portfolio
---

**Completed** - 2023 | MATLAB - Simulation - Decentralized Control - Control tuning and optimization 
<div class="project-github-link">
  <a href="https://github.com/AlePuglisi/three-tanks-distributed-control" class="btn btn--inverse">GitHub Repo</a>
</div> <br>
Final group project assignment of a course on [Networked Control systems](https://www11.ceda.polimi.it/schedaincarico/schedaincarico/controller/scheda_pubblica/SchedaPublic.do?&evn_default=evento&c_classe=810213&__pj0=0&__pj1=7f724b397a9ae97bd6cf089503f5774c).

In this project, we solve a benchmark problem in control theory, the (linearized) modeling and control of a system of three tanks in series.
In particular, coherently with the course topics, we implement different control schemes (centralized, decentralized, distributed).
Simulation and performance analysis are done both in continuous-time and discrete-time domains.

**Summary**:
- Modeled and Simulated a Three Tanks system dynamics in MATLAB.
- Implemented and Tuned Multi‐Variable Control structures, using Linear Matrix Inequalities solved with YALMIP
optimization toolbox, making the system five times faster and eliminating water oscillations.
- Improved controller performance with a rate limiter, reducing control action peak by a factor of ten, without losing
system speed.

Given the state-space model of a three-tank system:

**Objective**:
- Model the system in MATLAB and analyze its stability both in continuous and discrete time.
- Use the MATLAB optimization toolbox 'yalmip' to solve linear matrix inequality (LMI), and tune 
 different controller structure (in continuous and discrete time):
  - centralized
  - decentralized 
  - different distributed schemes
- Simulate the system. Analyze the performance and provide graphical results and quantitative 
 proof of the results' quality.

**Original Contribution**:
Because the control action often performs unrealistic steps, control rate limitations have been included (slides 69-82). 
To do so, a novel idea has been implemented: 
Defining an extended system model and new LMIs, with a cost function to limit control input magnitude and rate. 
With this approach, I obtain a 100% more realistic control action.

**Final Results**:
- Speed up the system, making it two times faster than the open loop dynamic. 
- Removed any waves (oscillations and overshoots) during settling time.
- Found the best choice of sampling time that doesn't degrade performances. 
- Provided a realistic interpretation of the results, considering the physical limitations of a real 
 system.

<iframe src="/files/projects/Three_Tanks_Report.pdf" width="100%" height="700" frameborder="no" border="0" marginwidth="0" marginheight="0"></iframe>