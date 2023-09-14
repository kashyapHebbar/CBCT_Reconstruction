
---

# Enhancing Cone Beam Computed Tomography (CBCT) Images through Deep Learning

## Table of Contents
1. [Introduction](#introduction)
2. [Objectives](#objectives)
3. [Methodology](#methodology)
4. [Prerequisites](#prerequisites)
5. [Installation](#installation)
6. [Usage](#usage)
7. [Results](#results)
8. [Future Work](#future-work)
9. [Contributing](#contributing)
10. [License](#license)

## Introduction
Traditional imaging techniques in Image-Guided Radiation Therapy (IGRT) often suffer from noise, artifacts, and limited contrast ranges. Specifically, Cone Beam Computed Tomography (CBCT), a low-cost but less reliable option than CT scans, needs enhancement to be more effectively used in medical procedures. This project addresses these challenges by implementing deep learning algorithms tailored for CBCT image quality enhancement.

## Objectives
- **Pre-Training on CT & CBCT Data**: Leverage Convolution Meets Masked Autoencoders (ConvMAE) to pre-train the model using high-quality CT and CBCT images, ensuring the model grasps the essential features from CT imaging.
- **Architect a Deep Learning Algorithm**: Develop an end-to-end deep learning model that incorporates Self-Supervised Learning and Generative Adversarial Networks to enhance CBCT images.
- **Performance Metrics**: Validate the algorithm's effectiveness using a comprehensive set of metrics including SNR, PSNR, and SSIM, as well as expert clinical evaluations.

## Methodology
- **Generative Adversarial Networks (GANs)**: Utilized to generate high-quality CBCT images, eliminating noise and improving contrast.
- **Composite Loss Functions**: Employ semantic consistency and style loss for fine-tuning the objective function.
- **Baseline Comparisons with Astra-Toolbox**: The performance of our model is rigorously compared against images created by Astra-Toolbox to evaluate its efficacy.

## Prerequisites
- Python 3.x
- PyTorch 1.x
- Astra-Toolbox
- Other dependencies can be found in `requirements.txt`

## Installation
Clone the repository and install the necessary packages:
```bash
git clone https://github.com/kashyapHebbar/CBCT_Reconstruction.git
cd CBCT_Reconstruction
pip install -r requirements.txt
```

## Usage
To run the program:
```bash
python main.py --options your-options
```

## Results
The developed algorithm significantly improves CBCT image quality, outperforming traditional methods and exceeding current clinical standards. It holds promise for improving the accuracy and reliability of IGRT in cancer treatment.

## Future Work
- Investigate the adaptability of the model for other medical imaging techniques.
- Incorporate real-world clinical evaluations to assess practical viability.
- Fine-tune the model for specific types of artifacts and noise.

## Contributing
Contributions are welcome! Please read the contributing guidelines and code of conduct before submitting a pull request or opening an issue.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

