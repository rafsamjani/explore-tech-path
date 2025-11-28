# AI-ML Learning Journey

[![Progress](https://img.shields.io/badge/Progress-25%25-brightgreen)](https://shields.io/)
[![GitHub stars](https://img.shields.io/github/stars/rafsamjani/explore-tech-path.svg)](https://github.com/rafsamjani/explore-tech-path/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/rafsamjani/explore-tech-path.svg)](https://github.com/rafsamjani/explore-tech-path/network)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> **Belajar AI/ML dari dasar matematika sampai proyek real-world** / *Learning AI/ML from mathematical foundations to real-world projects*

<div align="center">
  <p>Learning journey for beginners who want exposure while learning AI/ML</p>
</div>

## 📚 Table of Contents

- [Deskripsi / Description](#deskripsi--description)
- [Struktur Folder / Folder Structure](#struktur-folder--folder-structure)
- [Progress Tracker](#progress-tracker)
- [Quick Start](#quick-start)
- [Kontribusi / Contributing](#kontribusi--contributing)
- [Lisensi / License](#lisensi--license)

## Deskripsi / Description

Repository ini berisi perjalanan belajar Artificial Intelligence dan Machine Learning dari dasar matematika hingga proyek-proyek nyata. Cocok untuk pemula yang ingin belajar sambil eksplorasi konsep AI/ML secara mendalam.

*This repository contains an AI/ML learning journey from mathematical foundations to real-world projects. Perfect for beginners who want to learn while exploring AI/ML concepts deeply.*

## Struktur Folder / Folder Structure

```
AI-ML/
├── README.md                 # Roadmap visual + progress tracker
├── requirements.txt          # numpy torch sklearn opencv transformers
│
├── 01-Notes/                 # ✅ MATHEMATIKA DASAR (Minggu 1-2)
│   ├── 01-Aljabar-Linear/    # vektor → eigenvalue [SELESAI DULU]
│   ├── 02-Kalkulus/          # turunan → optimisasi
│   └── 03-Peluang/           # probabilitas → inferensial
│
├── 02-Projects/              # ✅ PPT TUGAS KULIAH (Minggu 3)
│
├── 03-Machine-Learning/      # ✅ SKLEARN CLASSICAL ML (Minggu 4)
│   ├── notes/
│   │   ├── 01-reinforcement-learning/
│   │   ├── 02-supervised-learning/
│   │   └── 03-unsupervised-learning/
│   └── projects/
│       ├── 01-reinforcement-learning/  # Q-Learning
│       ├── 02-supervised-examples/     # Regression/Classification
│       └── 03-unsupervised-examples/   # Clustering/PCA
│
├── 04-Deep-Learning/         # ✅ PYTORCH PROGRESSION (Minggu 5-7)
│   ├── notes/
│   │   ├── 01-perceptron/                # ← 06-perceptron
│   │   ├── 02-neural-networks-basics/    # ← 01/09-neural-networks
│   │   ├── 03-backpropagation/           # ← 07-backpropagation
│   │   ├── 04-activation-loss/           # ← 05/08-activation/loss
│   │   ├── 05-optimizers/                # ← 10-optimizers
│   │   ├── 06-regularization/            # ← 11-regularization
│   │   ├── 07-cnn/                       # ← 02-cnn
│   │   ├── 08-rnn/                       # ← 03-rnn
│   │   └── 09-transformers/              # ← 04-transformers
│   └── projects/                         # Basic → Advanced
│       ├── 02-multilayer-nn/             # MNIST nn.Module
│       ├── 03-pytorch-basics/            # DataLoader+Adam
│       ├── 04-convolutional-nn/          # CIFAR10 CNN
│       ├── 05-recurrent-nn/              # Text LSTM
│       ├── 06-text-generation/           # Simple GPT
│       ├── 07-object-detection/          # Image detection
│       ├── 08-image-classification/      # Classification tasks
│       └── 09-tensorflow-examples/       # TensorFlow examples
│
├── 05-Computer-Vision/       # ✅ OPENCV + DL (Minggu 8)
│   ├── notes/
│   │   ├── 01-image-processing-basics/   # ← 01/09-image-processing
│   │   ├── 02-filters/                   # ← 08-filters
│   │   ├── 03-convolution/               # ← 06-convolution
│   │   ├── 04-feature-extraction/        # ← 02/07-feature-extraction
│   │   ├── 05-cnn-architectures/         # ← 05-cnn-architectures
│   │   ├── 06-object-detection/          # ← 03-object-detection
│   │   ├── 07-image-segmentation/        # ← 04-segmentation
│   │   └── 08-advanced-image-processing/ # Advanced techniques
│   └── projects/
│       ├── 01-image-preprocessing/       # OpenCV basics
│       ├── 02-face-detection/            # Haar cascades
│       ├── 03-basic-cnn/                 # Custom CNN
│       ├── 04-image-classification/      # Transfer learning
│       ├── 05-object-detection/          # YOLO
│       ├── 06-object-tracking/           # SORT algorithm
│       └── 07-transfer-learning/         # Transfer learning techniques
│
└── 06-NLP/                   # ✅ TRANSFORMERS LAST (Minggu 9)
    ├── notes/
    │   ├── 01-text-preprocessing/         # ← 03-text-preprocessing
    │   ├── 02-n-grams/                    # ← 02-n-grams
    │   ├── 03-word-embeddings/            # ← 05-word-embeddings
    │   └── 04-language-models/            # ← 01/04-transformers
    └── projects/
        ├── 01-text-classification/        # TF-IDF + Logistic
        ├── 02-sentiment-analysis/         # LSTM sentiment
        ├── 03-named-entity-recognition/   # spaCy/BERT
        └── 04-translation/                # Helsinki-NLP
```

## Progress Tracker

| Topik / Topic | Status | Progress | Keterangan / Notes |
|---------------|--------|----------|-------------------|
| Matematika Dasar / Basic Math | ✏️ | 60% | Aljabar Linear, Kalkulus, Peluang |
| Machine Learning | 📚 | 30% | Supervised & Unsupervised Learning |
| Deep Learning | 📚 | 20% | Neural Networks & Backpropagation |
| Natural Language Processing | 📚 | 10% | Tokenization & Embeddings |
| Computer Vision | 📚 | 10% | CNN & Image Processing |
| Proyek Manual / Manual Projects | ✏️ | 40% | Implementasi tanpa library |
| Proyek Berbasis Library / Library Projects | ✅ | 80% | NumPy, Pandas, Scikit-learn |

> Keterangan / Legend: 📚 Belum (Not Started) | ✏️ Sedang (In Progress) | ✅ Selesai (Completed)

<details>
<summary>Deskripsi Subfolder / Subfolder Descriptions</summary>

- **Notes/**: Berisi catatan matematika dalam format LaTeX untuk dasar-dasar ML
- **Projects/**: Folder untuk menyimpan PPT atau tugas yang dikumpulkan
- **Machine-Learning/**: Materi dan proyek tentang algoritma ML klasik
- **Deep-Learning/**: Catatan dan implementasi neural networks
- **NLP/**: Natural Language Processing konsep dan proyek
- **Computer-Vision/**: Pengolahan citra dan visi komputer

</details>

## Preview Rumus Matematika / Mathematical Formula Preview

Berikut adalah contoh notasi matematika dalam LaTeX:

**Matriks / Matrix:**
```latex
\mathbf{A} = \begin{bmatrix}
a_{11} & a_{12} & \cdots & a_{1n} \\
a_{21} & a_{22} & \cdots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{m1} & a_{m2} & \cdots & a_{mn}
\end{bmatrix}
```

**Gradient:**
```latex
\nabla f(x, y, z) = \frac{\partial f}{\partial x}\mathbf{i} + \frac{\partial f}{\partial y}\mathbf{j} + \frac{\partial f}{\partial z}\mathbf{k}
```

## Quick Start

1. **Clone repository** / Clone the repository:
   ```bash
   git clone https://github.com/rafsamjani/explore-tech-path.git
   cd explore-tech-path/ai-ml
   ```

2. **Install dependencies** / Instal dependensi:
   ```bash
   pip install -r requirements.txt
   ```

   Contoh file `requirements.txt`:
   ```
   numpy>=1.21.0
   pandas>=1.3.0
   scikit-learn>=1.0.0
   matplotlib>=3.4.0
   seaborn>=0.11.0
   jupyter>=1.0.0
   scipy>=1.7.0
   sympy>=1.8
   torch>=1.9.0
   torchvision>=0.10.0
   tensorflow>=2.6.0
   nltk>=3.6
   spacy>=3.1.0
   opencv-python>=4.5.0
   ```

3. **Mulai belajar** / Start learning:
   ```bash
   jupyter notebook
   ```

## Catatan Pengembangan Pribadi / Personal Development Notes

Repository ini adalah dokumentasi perjalanan belajar pribadiku di bidang AI/ML. Aku bekerja sendiri, membangun semuanya dari awal sambil belajar. Setiap catatan, proyek, dan eksperimen disini merupakan bagian dari upayaku memahami konsep-konsep dasar hingga lanjutan dalam kecerdasan buatan dan machine learning.

*This repository is documentation of my personal learning journey in AI/ML. I'm working solo, building everything from scratch while learning. Each note, project, and experiment here is part of my effort to understand fundamental to advanced concepts in artificial intelligence and machine learning.*

### Tujuan Pembelajaran / Learning Goals

- Memahami matematika dasar yang mendasari algoritma ML
- Mengimplementasikan algoritma ML dari awal tanpa library
- Menguasai library populer seperti NumPy, Pandas, dan Scikit-learn
- Menjelajahi Deep Learning dan Neural Networks
- Menyelesaikan proyek-proyek end-to-end dari pra-pemrosesan hingga evaluasi model

## Kontribusi / Contributing

Meskipun ini adalah proyek pembelajaran pribadiku, kontribusi tetap dipersilakan! Jika kamu menemukan kesalahan, memiliki saran perbaikan, atau ingin berbagi pendekatan yang berbeda, kamu bisa:

1. Fork repository ini / Fork this repository
2. Buat branch fitur baru / Create a new feature branch: `git checkout -b fitur-baru`
3. Lakukan perubahan dan commit: `git commit -m 'Tambah fitur baru'`
4. Push ke branch: `git push origin fitur-baru`
5. Submit pull request

*Kontribusi yang saya cari:*
- Klarifikasi konsep matematika yang rumit
- Alternatif implementasi algoritma
- Sumber belajar tambahan
- Kode yang lebih efisien atau bersih

## Membuat requirements.txt

Untuk membuat file `requirements.txt` secara otomatis dari lingkungan Python yang kamu gunakan:

```bash
pip freeze > requirements.txt
```

Atau untuk hanya menyertakan paket yang diinstal secara eksplisit (bukan dependensi mereka):

```bash
pip list --format=freeze > requirements.txt
```

Kemudian kamu bisa mengedit file tersebut untuk menentukan versi minimum yang diperlukan.

## Lisensi / License

Proyek ini dilisensikan di bawah [MIT License](https://opensource.org/licenses/MIT). Jika kamu membuat file LICENSE, pastikan untuk menyertakan informasi berikut:

```
MIT License

Copyright (c) 2025 rafsamjani

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

*This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.*

## 🚀 Call to Action

Proyek ini merupakan dokumentasi perjalanan belajarku sendiri di bidang AI/ML. Aku bekerja sendiri, membangun semuanya dari awal sambil belajar. Jika kamu menemukan proyek ini bermanfaat atau ingin mengikuti perjalanan belajarku:

- ⭐ Berikan bintang di repository ini / Star this repository
- 🍴 Fork repository untuk pengembanganmu sendiri / Fork for your own development
- 📝 Tambahkan catatan atau proyekmu sendiri / Add your own notes or projects
- 🤝 Submit PR dengan perbaikan dan penjelasan tambahan / Submit PRs with improvements
- 💬 Beri masukan atau saran untuk topik yang ingin kamu pelajari juga / Give feedback or suggestions

Mari kita bersama-sama membangun sumber belajar AI/ML yang bermanfaat untuk komunitas!

*Let's build a helpful AI/ML learning resource for the community together!*