This repository contains the code and experimental setup for the paper:

A. Aghabagherloo, R. Gálvez, D. Preuveneers and B. Preneel, "Unveiling Illusionary Robust Features: A Novel Approach for Adversarial Defenses in Deep Neural Networks," in IEEE Access, vol. 13, pp. 154678-154694, 2025, doi: 10.1109/ACCESS.2025.3604636
.

📌 Overview

Deep Neural Networks (DNNs) are vulnerable to adversarial examples (AEs)—subtle perturbations that remain imperceptible to humans but mislead models.
While robust features have been proposed as a defense, our study shows that models trained on them remain vulnerable to AutoAttack and PGD-based attacks when attackers have full model knowledge.

We explore the susceptibility of robust models to illusionary robust features—features that appear robust but correlate with incorrect labels, causing vulnerabilities.
To mitigate this, we propose a novel robustification algorithm that generates a purified robust dataset, improving resilience against adversarial attacks.

📂 Repository Structure
├── robustification/  
│   └── Baseline implementations of existing robustification methods  
│
├── Susceptibility_of_robust_model/  
│   └── Experiments testing the susceptibility of robust models to PGD Attack  
│
├── autoattack/  
│   └── AutoAttack evaluation scripts and results  
│
├── Purified_robust_model/  
│   └── Proposed robustification algorithm (Purified Robust Dataset approach)  
│
└── README.md  

📊 Datasets

We use CIFAR-10, MNIST, and CINIC-10 for experiments:

CIFAR-10: 60,000 color images (32×32) across 10 classes (50k training, 10k test).

MNIST: 70,000 grayscale handwritten digit images (28×28).

CINIC-10: 270,000 images (CIFAR-10 + ImageNet samples), across the same 10 classes, for scalable robustness evaluation.

⚙️ Setup & Requirements

Clone the repository:

git clone https://github.com/alireza1375/Illusionary-Robust-Features.git
cd Illusionary-Robust-Features


📑 Citation

If you use this repository, please cite:

@article{Aghabagherloo2025Illusionary,
  author={Aghabagherloo, A. and Gálvez, R. and Preuveneers, D. and Preneel, B.},
  journal={IEEE Access}, 
  title={Unveiling Illusionary Robust Features: A Novel Approach for Adversarial Defenses in Deep Neural Networks}, 
  year={2025},
  volume={13},
  pages={154678-154694},
  doi={10.1109/ACCESS.2025.3604636}
}

🙌 Acknowledgements

CIFAR-10 dataset by Alex Krizhevsky.

MNIST dataset by Yann LeCun et al.

CINIC-10 dataset by Luke Darlow et al.

AutoAttack library by Francesco Croce and Matthias Hein.
