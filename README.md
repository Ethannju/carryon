<h1 align="center">Pack Light, CarryOn: Building Object-Oriented Context for Long-Horizon Agents</h1>

<p align="center">
  <a href="https://ethannju.github.io/carryon/"><img src="https://img.shields.io/badge/Project-Page-2d6bb1.svg" alt="Project Page"></a>
  <!-- arXiv: replace the next badge once available, e.g. <a href="https://arxiv.org/abs/XXXX.XXXXX"><img src="https://img.shields.io/badge/arXiv-XXXX.XXXXX-b31b1b.svg" alt="arXiv"></a> -->
  <img src="https://img.shields.io/badge/arXiv-coming%20soon-lightgrey.svg" alt="arXiv: coming soon">
</p>



https://github.com/user-attachments/assets/5f4a6889-5cf6-41a4-aff1-327a9d5d6b7b



CarryOn is a context runtime for long-horizon agents. Instead of replaying the
interaction history, it builds the agent's context around reusable **task
objects**: carriers for completed work, an execution context for what is left to
do, and a live tail of recent steps. With Claude Opus 4.7 on OSWorld 2.0, it
raises the partial score from 43.9% to 49.7% while cutting tokens by 52% and cost
by 36%.

<p align="center"><img src="docs/assets/overview.png" alt="Overview of CarryOn" width="860"></p>

## Results

<p align="center"><img src="docs/assets/osworld-results.png" alt="Task performance on OSWorld 2.0" width="760"></p>
<p align="center"><sub>Task performance on OSWorld 2.0. CarryOn improves both binary and partial
scores of the same Claude Opus 4.7 agent while cutting cost per task by 35.9%.
* Reproduced with the official benchmark and API.</sub></p>

<p align="center"><img src="docs/assets/context-and-cost.png" alt="Context and cost dynamics on OSWorld 2.0" width="760"></p>
<p align="center"><sub>Context and cost over agent turns on OSWorld 2.0. The baseline's input context keeps
growing past 200K tokens, while CarryOn's stays near 65K; by turn 500 the cumulative cost is 34.1% lower.</sub></p>

## Code

The code will be released after the review process.
