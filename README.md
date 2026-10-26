# Hi, I'm Nur 👋
 
ML/AI student focused on deep learning, optimization, and ML systems. I build models and learning systems from first principles to understand what happens underneath the abstractions.
 
---
 
## Education
 
**BSc Applied Computer Science and AI Sapienza University of Rome**
 
Finishing 3rd year (2024–2027). Coursework: Linear Algebra, Calculus, Probability, Statistics, Algorithms, Computer Architecture, AI and Machine Learning, AI Lab (Computer Vision and NLP), Data Management and Analysis, Deep Learning, Optimization.
 
---
 
## Projects


**[wifi-presence-detection](https://github.com/Nur2424/wifi-presence-detection)**

• Framed passive WiFi sensing as a one-class anomaly detection problem, motivated by the constraint that only one
occupancy class is reliably available at deployment time. Built a custom ESP32 sensing node in C (ESP-IDF) and
collected 376K+ CSI frames across 11 sessions to capture variation under real-world conditions.
• Identified RF amplitude drift across sessions (8–12 units, comparable in magnitude to the presence signal) as the
dominant factor limiting cross-session generalization during exploratory data analysis. Redesigned the evaluation
protocol with session-based splits to prevent leakage, explaining the gap between naive within-session evaluation
and realistic deployment performance.
• Ran a two-factor ablation (window size ×stride) across 5 model families (LR, OCSVM, FC Autoencoder, 1D CNN,
Transformer); found that sampling density dominates architecture choice (best: F1 0.9725, AUC 0.9835). Writing a
paper in IEEE format as first author, supervised by Prof. Daniele Avola.


**[tensorgrad](https://github.com/Nur2424/tensorgrad)**

• Derived tensor-level backward passes for matmul, softmax, cross_entropy, and layernorm from first principles of
matrix calculus (Jacobians, chain rule over tensor contractions) without referencing any existing autograd
implementation; verified each against PyTorch via central finite differences (ϵ=10−5, atol 10−4) before use in the
GPT.
• Trained a character-level GPT (3.21M parameters) on TinyShakespeare entirely without PyTorch; val NLL 1.8467 vs
PyTorch baseline 1.8381 (gap of 0.0085 nats, attributed to float64 vs. float32 precision after matching all other
hyperparameters). 50+ test cases cover every primitive op, closed-form AdamW (atol 10−9), and causal-mask
structure; all 44 gradient checks pass.

 
**[language-models-from-scratch](https://github.com/Nur2424/language-models-from-scratch)**

• Reproduced a six-model progression (bigram →MLP →deep MLP →WaveNet →Transformer), each architecture
addressing a limitation of the previous one; tracked val NLL as a consistent evaluation metric: 2.45 →2.16 →2.08
→1.99 (WaveNet-scaled, 76k params) / 2.02 (WaveNet-22k) →2.00 (Transformer).
• Diagnosed a silent BatchNorm bug: dim=0 on 3D (B,T,C) input computes per-timestep statistics and causes
running stats to accumulate incorrect shapes; dim=(0,1) is correct. Paired BuggyBatchNorm1d with the fixed version
for documentation. Chose Pre-LayerNorm over Post-LN on empirical gradient-stability grounds.


**[microgradplus](https://github.com/Nur2424/microgradplus)**

• Scalar reverse-mode autograd engine in pure Python (zero external dependencies); derived softmax backward
analytically via the CCE identity ∂L/∂zi = pi−yi and implemented through existing primitives. Includes Adam with
bias corrections (Kingma & Ba 2015), 4 loss functions, and Xavier/He init; 44/44 gradient checks pass and 95%
accuracy on Two Moons.
 
**[ml-network-analysis](https://github.com/Nur2424/ml-network-analysis)**

• Modelled the ML/AI open-source ecosystem as a co-contributor network of 500 GitHub repositories; clustering
coefficient 5.3×an Erd˝ os–Rényi null model, 11 Louvain communities (modularity Q=0.21). One chi-squared test
was abandoned when the minimum expected cell count fell to 0.29 and re-run on a restricted table.
• Pearson and Spearman correlations between degree centrality and log-star count were near zero (p>0.05),
corroborated by a t-test on core vs periphery splits (p=0.24). Network centrality showed little association with
repository popularity in the sampled data.

---
 
## Skills
 
Python · PyTorch · NumPy · Pandas · Matplotlib · NetworkX · Git
 
---
 
## Reach me
 
taabaldievnur06@gmail.com
