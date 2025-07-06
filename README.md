# 🧠 Task 4: Image-to-Image Translation with Pix2Pix (cGAN)

This project demonstrates how **Pix2Pix**, a Conditional Generative Adversarial Network (cGAN), performs **image-to-image translation** — a powerful technique that converts structured input images (like edges or sketches) into realistic outputs (like real shoes, facades, etc.).

---

## 🧾 What is Pix2Pix?

Pix2Pix is a deep learning model that learns to map input images to output images. It is particularly useful for tasks such as:
- Turning edge sketches into real images
- Converting black-and-white images to color
- Translating day-to-night photos, and more.

It uses two components:
- A **Generator**: Learns to create realistic images from input
- A **Discriminator**: Learns to distinguish real images from fake ones

They are trained together in a GAN framework.

---

## 🛠 What I Did in This Project

Due to resource limitations on Colab and the heavy compute requirements of Pix2Pix:

- I used a **preformatted input image** that simulates the Pix2Pix dataset structure (edges on the left, real photo on the right).
- I split this image into:
  - **Input image**: The edge sketch
  - **Target image**: The real counterpart (not used in inference here)
- I **simulated Pix2Pix translation** by applying a basic image operation (`invert`) to create an output image from the edge sketch.

---

## 🖼️ Input and Output

| Input (Edge Image) | Simulated Output |
|--------------------|------------------|
| ![Input](sample_pix2pix_input.jpg) | ![Output](generated_pix2pix_output.jpg) |

> ⚠️ *Note: Output is simulated due to hardware constraints. Actual Pix2Pix training or pretrained inference was not feasible within Colab's limits.*

---

## 📁 Files Included

- `prodigy_ga_04.ipynb`: Full Colab notebook
- `sample_pix2pix_input.jpg`: The input sample image used for the demo
- `generated_pix2pix_output.jpg`: Simulated output image
- `README.md`: Project documentation (this file)

---

## ✅ What This Project Demonstrates

- Understanding of conditional GANs (cGAN)
- How Pix2Pix works: input/output structure, model purpose
- Practical limitation handling using simulation
- Image preprocessing and basic augmentation steps in Python

---

## 📚 References

- [Pix2Pix Paper](https://arxiv.org/abs/1611.07004)
- [Official Pix2Pix Repo](https://github.com/phillipi/pix2pix)
- [CycleGAN + Pix2Pix PyTorch](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix)

---

✨ *Submitted as part of the Prodigy AI Internship — Task 4*
