# 🎨 Anime Autoencoder Playground

![GitHub Repo Size](https://img.shields.io/github/repo-size/FWKMultiverse/FWK-Multiverse)
![GitHub stars](https://img.shields.io/github/stars/FWKMultiverse/FWK-Multiverse)
![GitHub license](https://img.shields.io/github/license/FWKMultiverse/FWK-Multiverse)
![Python](https://img.shields.io/badge/python-3.11-blue)
![AI](https://img.shields.io/badge/AI-MultiAgent-green)

---

## 🚀 Project Overview

Welcome to the **Anime Autoencoder Playground**!  

This project is a **fun experimental AI demo** designed for learning and exploration purposes.  
It uses a **deep convolutional autoencoder** to generate anime-style images based on a small dataset downloaded from Google Images.  

⚠️ **Important:** This project is **not intended for production** or professional-level image generation.  
It is simply a **playground and example** to help you understand AI concepts and experiment with your own modifications.  

The autoencoder can:
- Learn from a small anime dataset (~30 images)
- Generate **new images** resembling the training data
- Work on **CPU or GPU** automatically
- Train incrementally for **progressive improvement**

---

## 🛠 Features

- Deep autoencoder for 512x512 images 🎨  
- Automatic GPU detection (GTX 1050 Ti or newer) ⚡  
- CPU fallback if no GPU is available 🖥  
- Incremental training using a **data generator** (reduces memory usage)  
- Fully open for **customization and experimentation** 🛠  
- Creates original outputs, not just copies of dataset images  

---

## 📂 Project Structure

```text
.
├── DataF/           # Downloaded dataset (~30 anime images)
├── Model/           # Trained autoencoder model
├── datapng/         # Generated images output
├── autoencoder.py   # Main Python script for training and generation
└── README.md        # Project documentation
⚡ Installation & Dependencies
Install required libraries via pip:

bash
คัดลอกโค้ด
python -m pip install --upgrade pip
python -m pip install tensorflow pillow google-api-python-client numpy requests
TensorFlow will automatically use your GPU if available, otherwise fallback to CPU.
Recommended RAM: ~6GB. CPU-only training works as well.

🏁 Usage
Clone the repository:

bash
คัดลอกโค้ด
git clone https://github.com/FWKMultiverse/AnimeAutoencoderPlayground.git
cd AnimeAutoencoderPlayground
Set up your Google API key and Custom Search Engine ID in the script:

python
คัดลอกโค้ด
GOOGLE_SEARCH_API_KEY = "YOUR_API_KEY"
GOOGLE_CSE_ID = "YOUR_CSE_ID"
Run the training and generation script:

bash
คัดลอกโค้ด
python autoencoder.py
After training, generated images will appear in the datapng/ folder.
You can continue training to improve image quality gradually.

📝 Notes
This project does not produce professional-quality anime images.

It's meant as a learning tool and a starting point for your own experiments.

Feel free to tweak model layers, batch size, epochs, or dataset for better results.

Only 30 images are used for demonstration purposes to limit memory usage.

🌐 Related Works
The main project I develop focuses on AI experiments and multi-agent systems:

FWK-Multiverse
A high-level AI project exploring autonomous agents and machine learning experiments.

💖 Support
If you enjoy my work and want to support me:

GitHub Sponsors

Your support helps me upgrade hardware, run AI experiments, and continue building projects. Every contribution means a lot! 🚀

📫 Contact
📧 Email: yoglawm644@gmail.com
🌐 Facebook Page: FWK Multiverse
🐦 Twitter/X: @FWK_Multiverse

⚡ License
This project is open-source and free to use, modify, and experiment with.
Feel free to adapt the code for your own projects, but remember it is just a playground/demo, not a professional-grade model.

🔧 Tags
Python TensorFlow AI Anime Autoencoder Deep Learning GPU CPU Experimental Learning Fun Demo
