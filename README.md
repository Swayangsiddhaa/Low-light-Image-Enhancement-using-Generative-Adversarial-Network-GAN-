# Low-light-Image-Enhancement-using-Generative-Adversarial-Network-GAN-

🌙 Low-Light Image Enhancement using Attention U-Net GAN ✨: - 

Welcome to the Attention U-Net GAN repository! This deep learning project is designed to transform extreme low-light photos into bright, clear, and photorealistic images.
Traditional image processing models (like standard CNNs) are fast but often produce blurry, "over-smoothed" images. On the other hand, modern generative models (like Diffusion) create beautiful textures but are too slow for real-time use. This project bridges that "Efficiency Gap" by delivering generative-grade realism in a fast, single-pass framework! 🚀

🧠 Architecture Overview: -

This model utilizes a Generative Adversarial Network (GAN) framework with two highly optimized components:-

1) ✨ The Generator (Attention U-Net): Built on an encoder-decoder backbone, this generator integrates Spatial Attention Gates. Instead of wasting computing power on empty dark noise, these gates act like a highlighter, forcing the AI to focus entirely on restoring complex structural edges and high-frequency details.
   
2) 🔍 The Discriminator (Markovian PatchGAN): Instead of grading the entire image with a single "Real/Fake" score, the PatchGAN evaluates the image in localized grids (e.g., 70x70 pixel patches). By grading the image piece-by-piece, the AI is mathematically forced to hallucinate and enforce highly realistic micro-textures across the entire photo.

📸 Dataset: -

This model is trained on the LOL (Low-Light) Dataset.
It utilizes paired standard RGB images, mapping extremely dark, noisy photos directly to their brightly lit, long-exposure ground-truth counterparts.

🌟 Key Outcomes & Benefits: -

Prevents Over-smoothing: The PatchGAN discriminator effectively eliminates the blurry look common in traditional low-light enhancement models.
Photorealistic Textures: Generates highly accurate micro-textures and sharp edges.
Highly Efficient: Designed to execute in a single forward pass, completely bypassing the heavy, iterative sampling delays of diffusion models. Perfect for fast, real-world applications! ⚡

🛠️ Tech Stack & Tools: -

Language: Python 🐍
Deep Learning Framework: PyTorch / TensorFlow (Update based on what you used)
Computer Vision: OpenCV, PIL, NumPy, Matplotlib
Concepts: Generative Adversarial Networks (GANs), Spatial Attention Mechanisms, Image RestorationIT License. See the LICENSE file for details.hoto.png --output ./results/
