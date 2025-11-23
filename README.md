# MIT Sports Analytics Paper Competition

## Overview
This repository accompanies the abstract submission for the MIT Sports Analytics Paper Competition. As discussed with Kelly Condon (MIT responsible for the competition), due to the high volume of submissions, abstracts may be submitted with a placeholder GitHub link. The full implementation and code will be provided at the full paper deadline.

## Repository Structure (to be updated)
project/

├── data/ # Public datasets

├── notebooks/ # Reproducibility workflows

└── README.md # Project documentation

## Data
- **Current submission**: uses synthetic/public placeholders.  
- **Full paper version**: will include adapted pipelines with publicly available data.  

## Instructions
For now, no runnable code is attached.  
Once the full paper is requested, this repository will be updated with:

- Preprocessing scripts  
- Core algorithm implementation  
- Reproducibility instructions  

---

## Abstract
In professional football, debates often focus on costs, revenues, wages, and titles, yet the dimension of efficiency—how much sporting or financial output is generated per euro invested—remains critically overlooked. Our preliminary analyses reveal that 98.3% of clubs are not profitable, and even fewer operate on the efficiency frontier, defined as the set of optimal allocations where performance and profitability cannot be simultaneously improved. Most organizations thus convert capital outlays into fewer wins or weaker financial results than theoretically achievable.

We formalize the Football Efficient Frontier as a concave, decreasing function ε in the (Profitability P, Win Rate W) space. Let C denote total expenditure (transfers + wages). Then sporting performance follows W = f(C), f'(C) > 0, f''(C) < 0 an increasing function with diminishing marginal returns, while profitability follows P = g(C), g'(C) < 0 , g''(C) < 0.  a decreasing function as costs escalate. Lets define the feasible set as:

F = {(P,W) = (g(C), f(C)) : C ≥ 0} ⊂ ℝ2 . Because f is strictly increasing and g is strictly decreasing, F  is a continuous, strictly decreasing curve in the (P,W)-plane. The efficient frontier Ɛ is the (upper) boundary of outcomes by the best allocation of C , Ɛ = {(P,W) / ∄ (P',W') where P' ≥ P & W'≥ W}.

From this structure, two principal use cases emerge. Case 1: Maximize Wins subject to a given profitability (for ex P ≥ Pmin). This corresponds to elite clubs whose objective is sporting dominance while maintaining financial sustainability. Their optimal solution is located on ε at the point of maximum W given P ≥ 0. Case 2: Maximize Profit subject to a minimum win rate (W ≥ Wmin). This applies to mid-tier or development-oriented clubs, for which ensuring survival (e.g., Wmin = 40% to remain in the top division) is paramount. Here, the optimal solution lies on ε where profitability is maximized conditional on the sporting threshold.

Empirical validation illustrates the model’s utility. In a case study conducted for Reading FC, the club’s efficiency was benchmarked against neighboring teams in the English Championship. Results indicate a significant gap from the efficient frontier, underscoring suboptimal capital allocation in relation to both win rate and net financial balance. This research contributes by (i) mathematically defining football’s efficient frontier, (ii) contextualizing two practical use cases for strategic decision-making, and (iii) demonstrating through real-club data that current practices systematically underperform relative to optimal allocations. By bridging financial theory, performance analytics, and empirical case studies, the Football Efficient Frontier offers a replicable framework to guide squad optimization, ensuring rational trade-offs between profitability and sporting success.
