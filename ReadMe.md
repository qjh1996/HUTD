# Nearshore Underwater Target Detection Meets UAV-borne Hyperspectral Remote Sensing: A Novel Hybrid-level Contrastive Learning Framework and Benchmark Dataset&#x20;

## 📌 Overview

This repository contains the implementation of **HUCLNet**, a novel approach for hyperspectral underwater target detection (HUTD) and a novel HUTD benchmark dataset, **ATR2-UTR**.

## 📝 Abstract

UAV-borne hyperspectral remote sensing has emerged as a promising approach for underwater target detection (UTD). However, its effectiveness is hindered by spectral distortions in nearshore environments, which compromise the accuracy of traditional hyperspectral UTD (HUTD) methods that rely on bathymetric model. These distortions lead to significant uncertainty in target and background spectra, challenging the detection process. To address this, we propose the Hyperspectral Underwater Contrastive Learning Network (HUCLNet), a novel framework that integrates contrastive learning with a self-paced learning paradigm for robust HUTD in nearshore regions. HUCLNet extracts discriminative features from distorted hyperspectral data through contrastive learning, while the self-paced learning strategy selectively prioritizes the most informative samples. Additionally, a reliability-guided clustering strategy enhances the robustness of learned representations. To evaluate the method effectiveness, we conduct a novel nearshore HUTD benchmark dataset, ATR2-HUTD, covering three diverse scenarios with varying water types and turbidity, and target types. Extensive experiments demonstrate that HUCLNet significantly outperforms state-of-the-art methods. 

## 🚀 Methodology

### 🔹 Highlights

- **[Reliability-guided clustering strategy]**: This strategy assigns hyperspectral pixels to prototypes via unsupervised clustering, incorporating a fixed prototype derived from the reference spectrum.  A novel reliability criterion is introduced to assess cluster trustworthiness, refining pixel assignments into reliable clusters and unreliable instances.
- **[Hybrid-level Contrastive Learning Framework]**: The framework processes unreliable instances via instance-level contrastive learning to enhance discriminative representation and clustering accuracy, while reliable clusters undergo prototype-level contrastive learning to align target spectra with references while maintaining separation from background spectra.
- **[Integration of Self-Paced Learning (SPL)]**: HUCLNet introduces a self-paced learning paradigm that progressively refines the learning process by incorporating unreliable instances into reliable clusters as the model improves, enhancing representation learning and overall performance in HUTD.

### 🏗 Framework

The figure below illustrates the overall pipeline of our method:

![A3](Figures\A3.jpg)

## 📊 Dataset

We introduce ATR2-HUTD, a new dataset designed for HUTD. The ATR2-HUTD dataset, comprising three sub-datasets collected from diverse aquatic environments (lake, river, and sea), addresses scene diversity limitations and data size constraints by offering larger image dimensions (up to 3536×6403536×640 pixels) and enhanced spatial details, thereby improving model generalization and robustness for real-world hyperspectral underwater target detection tasks.

### 🔽 Download

You can download the dataset from the following links:

- [Google Drive](https://drive.google.com/file/d/1AdwWVHvlGHBDSmWQUZ_ziWz8Fk7JV0NG/view?usp=sharing)
- [Baidu Cloud](https://pan.baidu.com/s/1bhDyOUELXLKf85y_NT-smw?pwd=s45g) (Password: `s45g`)

## ⏳ Code Release

The source code will be made publicly available upon the acceptance of our paper. Stay tuned for updates!

## 🔗 Citation

If you find our work helpful, please consider citing:

```bibtex
@article{your_paper,
  title   = {Your Paper Title},
  author  = {Your Name and Co-authors},
  journal = {Journal Name},
  year    = {YYYY},
  volume  = {XX},
  pages   = {XX-XX},
  doi     = {XX.XXXX/XXXXXXX}
}
```

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📬 Contact

For any questions, feel free to reach out:

- 📧 Email: [qijiahao1996@nudt.edu.cn](mailto\:qijiahao1996@nudt.edu.cn)
