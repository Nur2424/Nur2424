# Hi, I'm Nur 👋
 
ML/AI student focused on deep learning, optimization, and ML systems. I build models and learning systems from first principles to understand what happens underneath the abstractions.
 
---
 
## Education
 
**BSc Applied Computer Science and AI Sapienza University of Rome**
 
Finishing 3rd year (2024–2027). Coursework: Linear Algebra, Calculus, Probability, Statistics, Algorithms, Computer Architecture, AI and Machine Learning, AI Lab (Computer Vision and NLP), Data Management and Analysis, Deep Learning, Optimization.
 
---
 
## Projects
 
**[microgradplus](https://github.com/Nur2424/microgradplus)**
Scalar autograd engine and neural network library built from scratch in pure Python with zero dependencies. Implements reverse-mode automatic differentiation, backpropagation, activations, losses (MSE, BCE, hinge, categorical cross-entropy with softmax), and optimizers (SGD with momentum, Adam with bias correction derived analytically). Every gradient verified against PyTorch with 44 tests using finite-difference approximation.

**[tensorgrad](https://github.com/Nur2424/tensorgrad)**
Tensor-level autograd engine built from scratch in NumPy the natural extension of microgradplus from scalar to matrix operations. Hand-derived gradients for matmul, softmax, cross-entropy, and layer norm. Trains a character-level GPT on Shakespeare without PyTorch: val loss 1.8467 vs PyTorch's 1.8381, difference 0.0085.
 
**[language-models-from-scratch](https://github.com/Nur2424/language-models-from-scratch)**
Character-level language models progressing from bigram counting statistics to a GPT-style Transformer, all trained on the same 32k names dataset with the same evaluation metric. Six models, each fixing a concrete limitation of the previous one: bigram (NLL 2.45) -> MLP -> deep MLP with BatchNorm -> WaveNet -> Transformer (NLL 2.00). Includes runnable scripts, derivation notebooks, and a reusable training diagnostics module.
 
**[wifi-presence-detection](https://github.com/Nur2424/wifi-presence-detection)**
WiFi Channel State Information (CSI) based indoor presence detection, framed as anomaly detection across a three phase empirical study. Built a custom ESP32-WROOM-32 sensing node collecting CSI at ~80 Hz across 51 active subcarriers, with a Python logger writing raw amplitude data to CSV. Feature engineering extracts 55 per-frame features (51 subcarrier amplitudes + mean, std, max, energy), aggregated with mean and standard deviation pooling into 110-dimensional window vectors. Evaluated five architectures Logistic Regression, OCSVM, FC Autoencoder, 1D CNN, and Transformer across four temporal window sizes (12.5 ms to 10 s) under both non-overlapping and stride-1 overlapping training conditions. Primary dataset: 376,514 CSI frames across 11 sessions on two days, with a cross day amplitude drift of 8–12 units comparable in magnitude to the occupancy signal itself. Key findings: training window sampling density is a stronger performance lever than architecture choice shifting from non-overlapping to stride-1 overlapping windows improves F1 by up to +0.160 (LR, W4) and +0.136 (CNN, W2), one-class methods generalize more robustly under cross session conditions (Conv AE AUC 0.747 vs. LR AUC 0.640 in feasibility phase), OCSVM uniquely degrades under long window overlapping, consistent with near-duplicate training points inflating one-class boundary geometry. Best configurations: FC Autoencoder F1 0.9725 / AUC 0.9835, 1D CNN F1 0.9612 / AUC 0.9857.
 
**[ml-network-analysis](https://github.com/Nur2424/ml-network-analysis)**
Network science analysis of 500 top ML/AI GitHub repositories. Bipartite contributor-repository graph, Louvain community detection (modularity Q=0.21), centrality analysis, and hypothesis testing. Key finding: network centrality does not predict repository popularity (p=0.24).

---
 
## Skills
 
Python · PyTorch · NumPy · Pandas · Matplotlib · NetworkX · Git
 
---
 
## Reach me
 
taabaldievnur06@gmail.com
