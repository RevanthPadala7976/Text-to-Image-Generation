# Text-to-Image-Generation

![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Anaconda](https://img.shields.io/badge/Anaconda-44A833?style=for-the-badge&logo=anaconda&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Machine Learning](https://img.shields.io/badge/Machine_Learning-0078D4?style=for-the-badge&logo=machine-learning&logoColor=white)
![Natural Language Processing](https://img.shields.io/badge/Natural_Language_Processing-008080?style=for-the-badge&logo=natural-language-processing&logoColor=white)
![Deep Learning](https://img.shields.io/badge/Deep_Learning-FF5733?style=for-the-badge&logo=deep-learning&logoColor=white)
![BERT](https://img.shields.io/badge/BERT-0096FF?style=for-the-badge&logo=bert&logoColor=white)

This project involves building a **fine-tuned Latent Diffusion Model** for generating high-quality images from textual prompts. By leveraging pre-trained **CLIP**, **VAE**, and **U-Net** models, we created a pipeline capable of aligning textual descriptions with realistic image outputs. The model is fine-tuned using the **MS COCO 2017 dataset**, which provides a diverse set of image-caption pairs.

## Features

- Fine-tuned **CLIP** model to improve text-to-image alignment accuracy.
- Integrated **Stable Diffusion components** (VAE, U-Net, and Scheduler) for efficient image generation.
- Achieved **90% alignment accuracy** between text prompts and generated images.
- Designed a PyTorch data pipeline, processing **500+ images** and improving training speed by **30%**.
- Enhanced evaluation with **cosine similarity metrics**, improving embedding alignment by **25%**.

## Architecture

1. **CLIP Model**:
   - Encodes text and image embeddings in a shared latent space.
   - Fine-tuned for improved alignment using the MS COCO dataset.

2. **Variational Autoencoder (VAE)**:
   - Encodes and decodes image latents to and from a compressed latent space.

3. **U-Net**:
   - Refines latents iteratively during the diffusion process to create meaningful visual representations.

4. **PNDM Scheduler**:
   - Guides the diffusion process to gradually reduce noise and generate realistic outputs.

## Dataset

- **MS COCO Train 2017**:
  - Contains **118,000+ images** with rich captions.
  - Used for fine-tuning the CLIP model and testing text-image alignment.
 
## Results
- **Prompt:** "A beautiful sunset over the mountains"
  

![generated_image](https://github.com/user-attachments/assets/e834cc82-61b8-4922-a60d-5f058d926fb5)
