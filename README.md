# FILLER---Stack-Overflow-title-generator
This is my implementation for "Good things come in three: Generating SO Post Titles with Pre-Trained Models, Self Improvement and Post Ranking" https://arxiv.org/abs/2406.15633

The paper introduces FILLER, a novel approach for automatically generating high‑quality titles for Stack Overflow posts. Overall, It give out a significant better result compare to past paper on this same problem.

The process has three main stages: first, a fine‑tuning stage where a pre‑trained language model (CodeT5) is adapted using bi‑modal inputs that combine code snippets and textual descriptions across multiple programming languages; second, a self‑improvement stage where the model’s own predictions are fed back into training to reduce exposure bias and help it learn from its mistakes; and third, an inference stage that generates multiple candidate titles and applies a post‑ranking method (using TextRank) to select the most relevant and informative one.

I've changing the post-ranking method from TextRank to MMR for better choosing among candidates.
