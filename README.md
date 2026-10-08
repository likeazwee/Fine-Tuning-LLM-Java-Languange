# Fine-Tuning LLM Bahasa Jawa Menggunakan Infrastruktur HPC / Cloud (Google Colab)

Repositort ini berisi implementasi studi kasus untuk tugas kuliah yang mengadopsi konsep dari materi kuliah umum **"Bridging Global Infrastructure to Address Local Challenge with HPC"** oleh Asst. Prof. Dr. Worawan Diaz Carballo. 

Proyek ini mendemonstrasikan bagaimana peran seorang **"Integrator"** dapat menjembatani sumber daya komputasi modern (seperti High-Performance Computing atau Google Colab GPU) untuk menyelesaikan tantangan lokal, khususnya dalam pemrosesan bahasa alami (*Natural Language Processing*) untuk bahasa daerah di Indonesia (Studi Kasus: **Bahasa Jawa**).

---

## 📌 Latar Belakang & Motivasi
Di era digital, infrastruktur global berskala raksasa seperti *High-Performance Computing* (HPC) dan arsitektur *Large Language Model* (LLM) umumnya dikembangkan untuk bahasa-bahasa mayoritas (*high-resource languages*). Tantangan nyata di tingkat lokal adalah bagaimana memanfaatkan daya komputasi tersebut untuk melestarikan dan mengembangkan teknologi berbasis bahasa daerah (*low-resource languages*), salah satunya Bahasa Jawa, guna mendukung inklusivitas digital dan pelestarian budaya.

Karena pelatihan model bahasa berskala besar membutuhkan sumber daya komputasi masif, proyek ini menggunakan pendekatan **Parameter-Efficient Fine-Tuning (PEFT/LoRA)** yang dieksekusi di atas akselerator GPU.

---

## 🛠️ Teknologi & Tools yang Digunakan
*   **Bahasa Pemrograman:** Python
*   **Deep Learning Framework:** PyTorch & Hugging Face Transformers
*   **Metodologi Efisiensi:** PEFT (Parameter-Efficient Fine-Tuning) dengan **LoRA** (*Low-Rank Adaptation*)
*   **Training Helper:** TRL (`SFTTrainer` & `SFTConfig`)
*   **Dataset:** IndoNLP/NusaX-senti (Subset Bahasa Jawa / `jav`)
*   **Infrastruktur Komputasi:** Google Colab (GPU T4) / Skrip Batch HPC (Slurm)

---

## 🚀 Cara Menjalankan Proyek (Quick Start)

Anda dapat menjalankan proyek ini langsung melalui **Google Colab** dengan memanfaatkan GPU gratis yang disediakan.

### 1. Prasyarat & Instalasi Library
Jalankan perintah berikut di dalam *cell* Google Colab Anda:
```python
!pip install --upgrade transformers peft trl liger-kernel torchao
!pip install "datasets<2.20.0"
```
---

## 👥 Kontributor & Referensi
* **Materi Kuliah Umum:** *Bridging Global Infrastructure to Address Local Challenge with HPC* oleh Asst. Prof. Dr. Worawan Diaz Carballo.
* **Dataset:** IndoNLP (`IndoNLP/NusaX-senti`).
