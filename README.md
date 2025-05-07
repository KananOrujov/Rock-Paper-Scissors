🧪 Approach 5: Synthetic Time Series Generation with Differential Privacy
📋 Project Description
This project investigates privacy-preserving synthetic time series generation using two deep learning models enhanced with Differential Privacy (DP): DP-GAN and DP-TimeGAN. The goal is to generate synthetic sequences that maintain the statistical properties of the original data while offering formal privacy guarantees.

This work was contributed by Kanan Orujov, focusing on integrating DP techniques into generative models for sequence data.

🔁 Repeatable Experiment: Step-by-Step Instructions
📦 Environment Setup
Install required libraries:

<pre> bash pip install torch opacus pandas numpy scikit-learn matplotlib </pre>
Ensure you're using Python 3.8+.

⚙️ Technologies Used
Python 3.8+

PyTorch

Opacus (for Differential Privacy in PyTorch)

Pandas

NumPy

scikit-learn

Matplotlib

🧠 Model Design
DP-GAN
Architecture: MLP-based Generator and Discriminator.

Privacy Mechanism: Integrated via Opacus using DP-SGD.

DP-TimeGAN
Architecture:

GRU-based components: Embedder, Recovery, Generator, Supervisor

Discriminator using DP-SGD

Adapted from: Original TimeGAN with added differential privacy constraints.

🏋️ Training
Phase 1: Autoencoder pre-training for sequence embedding.

Phase 2: Adversarial training with Differential Privacy.

Parameters used:

ε (epsilon) = 10.0

δ (delta) = 1e-5

📈 Evaluation
Visual Comparison: Real vs Synthetic time series plots.

Privacy Verification: Ensured privacy budget was not exceeded.

Metrics:

Similarity in temporal trends

Statistical fidelity

Measured ε and δ compliance

👤 Author
Kanan Orujov — Contributed the privacy-preserving synthetic time series generation using DP-GAN and DP-TimeGAN models.

📚 References
Yoon, J. et al. TimeGAN: Time-series Generative Adversarial Networks

Abadi, M. et al. Deep Learning with Differential Privacy

Goodfellow, I. et al. Generative Adversarial Nets
