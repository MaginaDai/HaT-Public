# HaT: Learning System Expansion with Efficient Heterogeneity-aware Knowledge Transfer

This repository contains the official implementation of **HaT**, a general and efficient framework for **learning system expansion** — a practical problem where AI systems must continuously incorporate new domains (e.g., users, devices, environments) under **label scarcity**, **data heterogeneity**, and **device constraints**.

HaT is designed for real-world, large-scale deployments where training a customized model for each new domain from scratch is prohibitively expensive. Instead, HaT selectively reuses and transfers knowledge from existing heterogeneous models to efficiently construct high-quality models for newly joined domains.

---

## 🚀 Key Ideas

HaT addresses learning system expansion through three core designs:

1. **Efficient Source Model Selection**  
   HaT filters and selects a small subset of high-quality source models using lightweight statistical features and representation similarity, significantly reducing communication and computation overhead.

2. **Sample-wise Knowledge Fusion**  
   Instead of assuming perfect teachers, HaT fuses predictions from multiple *imperfect and heterogeneous* source models using an attention-based mixer that assigns sample-specific weights.

3. **Adaptive Knowledge Injection**  
   A quality-verified knowledge dictionary stabilizes training by injecting only reliable fused predictions into the target model, with adaptive distillation strength based on knowledge quality.

Together, these designs allow HaT to expand learning systems **accurately**, **efficiently**, and **scalably**.

---

## 📊 Results Highlights

Across multiple tasks and modalities (IMU sensing, vision, EMG, audio, and multimodal activity recognition), HaT:

- Achieves **up to +16.5% accuracy improvement** over state-of-the-art baselines
- Reduces **training time by up to 31.1%**
- Cuts **communication traffic by up to 93.0%**
- Supports **heterogeneous model architectures** and **multi-round system expansion**

---

## 🧩 Applications

HaT is applicable to a wide range of real-world scenarios, including:

- Personalized mobile and wearable sensing
- Edge AI model customization
- Continual deployment of AI services across users and devices
- Resource-constrained and privacy-sensitive environments

---

## 📦 Code Release
The code will be released by **January 30** due to conflicting commitments.

## 📖 Citation

If you find this work useful, please consider citing:

```bibtex
@article{dai2024expand,
  title={Learning System Expansion with Efficient Heterogeneity-aware Knowledge Transfer},
  author={Dai, Gaole and Xu, Huatao and Yang, Yifan and Tan, Rui and Li, Mo},
  journal={arXiv preprint arXiv:2412.04060},
  year={2024}
}

