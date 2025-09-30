# 🎨 Anime Autoencoder Playground – by a 16-Year-Old Enthusiast

![GitHub Repo Size](https://img.shields.io/github/repo-size/FWKMultiverse/FWK-Multiverse)
![GitHub stars](https://img.shields.io/github/stars/FWKMultiverse/FWK-Multiverse)
![GitHub license](https://img.shields.io/github/license/FWKMultiverse/FWK-Multiverse)
![Python](https://img.shields.io/badge/python-3.11-blue)
![AI](https://img.shields.io/badge/AI-DeepLearning-green)

---

## 🌟 Introduction

Welcome! This project is a **fun, experimental AI project** created by a **16-year-old enthusiast**.  
The goal is to explore **image generation using deep autoencoders** trained on anime images.

> ⚠️ **Disclaimer:**  
> This project is purely for **learning and experimentation**.  
> Models are simple, training is short, and outputs are illustrative.  
> Feel free to **customize, extend, and experiment** – this is meant as a **playground**. 😎  
> The results are not production-grade and mainly serve as a **guideline/example**.

---

## 📂 File Structure

├── DataF/ # Downloaded anime images (~30 images)
├── Model/ # Saved autoencoder model
├── datapng/ # Generated sample images
├── main.py # Main training and generation script
└── README.md # This README file

markdown
คัดลอกโค้ด

---

## ⚙️ How It Works – Step by Step

### 1️⃣ Fetch Images
- Uses **Google Custom Search API**  
- Queries: `"anime character"`, `"anime background"`, `"anime scenery"`  
- Downloads ~30 images into `DataF/`

### 2️⃣ Data Preprocessing
- Resize images to **512×512 pixels**  
- Normalize pixel values to **[0,1]**  
- Automatically **skip corrupted files**

### 3️⃣ Build Autoencoder
- **Encoder:** 3× Conv2D + MaxPooling layers  
- **Decoder:** 3× Conv2D + UpSampling layers  
- Output: reconstructed RGB image

### 4️⃣ Training
- Loss: **Mean Squared Error (MSE)**  
- Optimizer: **Adam**  
- Batch size: 1  
- Shuffle dataset every epoch  
- Trains for 20 epochs (simple/fun experiment)

### 5️⃣ Save Model
- Model saved to `Model/autoencoder_anime_512.h5`

### 6️⃣ Generate Image
- Decode a batch from trained autoencoder  
- Save output to `datapng/generated_anime_512.png`

---

## 🛠️ Customization & Tips

- Change queries to fetch different types of images  
- Increase dataset size for better quality  
- Modify encoder/decoder layers for deeper/wider architecture  
- Experiment with **data augmentation** or other generative models (GANs, VQ-VAE)  
- **Feel free to fork and adjust** this project to your liking

---

## 💖 Support Me on GitHub Sponsors

If you enjoy this project, support me here:

[![Sponsor](https://img.shields.io/badge/Sponsor-GitHub-green)](https://github.com/sponsors/FWKMultiverse)  
Or click directly: [https://github.com/sponsors/FWKMultiverse](https://github.com/sponsors/FWKMultiverse)

Your support helps me **upgrade hardware, run AI experiments, and continue building projects**. Every contribution means a lot! 🚀

---

## 📬 Contact

- 📧 Email: [yoglawm644@gmail.com](mailto:yoglawm644@gmail.com)  
- 🌐 Facebook Page: [FWK Multiverse](https://www.facebook.com/FWKMultiverse/)  
- 🐦 Twitter/X: [@FWK_Multiverse](https://x.com/FWK_Multiverse)

---

## 🏷️ Tags & Topics

`AI` `Deep Learning` `Autoencoder` `Anime` `Image Generation` `Python` `TensorFlow` `Experiment` `Playground` `Beginner-Friendly`

---

## ⚡ Summary

- **Purpose:** Learning AI image generation through a fun playground project  
- **Not production-grade:** Intended as a simple example for learning  
- **Codebase:** Easy to adapt, extend, and experiment with  
- **Audience:** Beginners, hobbyists, students, or anyone curious about AI  

🎉 Enjoy exploring AI, and feel free to fork, modify, and experiment!  
Remember: this is a **learning playground**, results are simple but fun. 😎
