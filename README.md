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
Unsupervised human presence detection from indoor sensor signals, framed as anomaly detection. Three models trained only on empty-room data and compared under a single experimental protocol: Isolation Forest, MLP autoencoder, and CNN autoencoder. CNN achieves F1 0.919 and recall 0.988. Built for the Sapienza AI Lab course with an IEEE-format paper.
 
**[ml-network-analysis](https://github.com/Nur2424/ml-network-analysis)**
Network science analysis of 500 top ML/AI GitHub repositories. Bipartite contributor-repository graph, Louvain community detection (modularity Q=0.21), centrality analysis, and hypothesis testing. Key finding: network centrality does not predict repository popularity (p=0.24).

---
 
## Skills
 
Python · PyTorch · NumPy · Pandas · Matplotlib · NetworkX · Git
 
---
 
## Reach me
 
taabaldievnur06@gmail.com
