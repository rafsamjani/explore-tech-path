# Vektor dan Skalar dalam Aljabar Linear

## Pendahuluan

Aljabar linear adalah cabang matematika yang sangat penting dalam ilmu komputer, khususnya dalam bidang Machine Learning dan Artificial Intelligence. Konsep dasar seperti vektor dan skalar merupakan fondasi utama yang harus dipahami sebelum melangkah ke konsep-konsep yang lebih kompleks seperti matriks, ruang vektor, dan transformasi linear.

Dokumen ini akan membahas secara mendalam tentang vektor dan skalar, disertai dengan contoh dan latihan untuk memperkuat pemahaman.

## Pengertian Dasar

### Skalar

Skalar adalah besaran yang hanya memiliki **nilai** atau **magnitude** saja, tanpa arah. Skalar merupakan bilangan tunggal yang digunakan untuk merepresentasikan kuantitas tertentu seperti panjang, waktu, suhu, atau massa.

**Contoh skalar:**
- Suhu ruangan: 25°C
- Tinggi badan: 175 cm
- Waktu perjalanan: 2 jam
- Berat benda: 50 kg

Dalam konteks aljabar linear dan komputasi, skalar biasanya direpresentasikan sebagai bilangan tunggal:

`s ∈ ℝ`

di mana ℝ adalah himpunan bilangan real.

### Vektor

Vektor adalah besaran yang memiliki **nilai** (magnitude) dan **arah**. Vektor sangat penting dalam ilmu komputer dan Machine Learning karena digunakan untuk merepresentasikan data, fitur, dan parameter model.

**Contoh vektor:**
- Kecepatan mobil: 60 km/jam ke arah timur
- Koordinat dalam ruang: (3, 4) atau (1, 2, 5)
- Fitur gambar dalam Machine Learning
- Parameter dalam model regresi

#### Representasi Vektor

Secara matematis, vektor biasanya ditulis dalam bentuk kolom:

```
v = [v₁]
    [v₂]
    [⋮ ]
    [vₙ]
```

atau dalam bentuk baris:

```
v = [v₁  v₂  ⋯  vₙ]
```

Kita juga sering melambangkan vektor dengan huruf kecil tebal:

```
v = [v₁]
    [v₂]
    [⋮ ]
    [vₙ]
```

**Contoh vektor 2D:**
```
v = [3]
    [4]
```

**Contoh vektor 3D:**
```
w = [1]
    [2]
    [5]
```

## Operasi pada Vektor dan Skalar

### Penjumlahan dan Pengurangan

#### Operasi antara Vektor dan Skalar

Kita dapat menambahkan atau mengurangkan skalar ke setiap elemen vektor. Misalnya, jika:

```
v = [v₁]
    [v₂]
    [⋮ ]
    [vₙ]
```

dan `s` adalah skalar, maka:

```
v + s = [v₁ + s]
        [v₂ + s]
        [  ⋮  ]
        [vₙ + s]

v - s = [v₁ - s]
        [v₂ - s]
        [  ⋮  ]
        [vₙ - s]
```

**Contoh:**
```
v = [1]    s = 5
    [2]
    [3]

v + s = [1 + 5] = [6]
        [2 + 5]   [7]
        [3 + 5]   [8]
```

#### Operasi antara Dua Vektor

Dua vektor dengan dimensi yang sama dapat dijumlahkan atau dikurangkan secara elemen per elemen:

```
u = [u₁]     v = [v₁]
    [u₂]         [v₂]
    [⋮ ]         [⋮ ]
    [uₙ]         [vₙ]
```

```
u + v = [u₁ + v₁]
        [u₂ + v₂]
        [   ⋮   ]
        [uₙ + vₙ]

u - v = [u₁ - v₁]
        [u₂ - v₂]
        [   ⋮   ]
        [uₙ - vₙ]
```

**Contoh:**
```
u = [1]     v = [4]
    [2]         [5]
    [3]         [6]

u + v = [1 + 4] = [5]
        [2 + 5]   [7]
        [3 + 6]   [9]
```

### Perkalian

#### Perkalian Skalar dengan Vektor

Ketika kita mengalikan sebuah vektor dengan skalar, kita mengalikan setiap elemen vektor dengan skalar tersebut:

```
s · v = s · [v₁] = [s · v₁]
            [v₂]   [s · v₂]
            [⋮ ]   [  ⋮  ]
            [vₙ]   [s · vₙ]
```

**Contoh:**
```
v = [2]    s = 4
    [3]
    [1]

s · v = 4 · [2] = [8]
            [3]   [12]
            [1]   [4]
```

#### Perkalian Dua Vektor

Ada beberapa jenis perkalian antara dua vektor. Dua yang paling umum adalah:

1. **Dot Product (Perkalian Titik)**: Menghasilkan skalar
2. **Cross Product (Perkalian Silang)**: Menghasilkan vektor (hanya dalam 3 dimensi)

##### Dot Product

Dot product dari dua vektor dengan dimensi yang sama didefinisikan sebagai:

`u · v = Σ(i=1 to n) uᵢ · vᵢ = u₁v₁ + u₂v₂ + ⋯ + uₙvₙ`

**Contoh:**
```
u = [1]     v = [4]
    [2]         [5]
    [3]         [6]

u · v = (1 · 4) + (2 · 5) + (3 · 6) = 4 + 10 + 18 = 32
```

##### Cross Product (hanya 3 dimensi)

Cross product dari dua vektor 3 dimensi didefinisikan sebagai:

```
u × v = [u₂v₃ - u₃v₂]
        [u₃v₁ - u₁v₃]
        [u₁v₂ - u₂v₁]
```

**Contoh:**
```
u = [1]     v = [4]
    [2]         [5]
    [3]         [6]

u × v = [(2 · 6) - (3 · 5)]   [-3]
        [(3 · 4) - (1 · 6)] = [ 6]
        [(1 · 5) - (2 · 4)]   [-3]
```

## Norma Vektor

Norma (atau magnitude) dari sebuah vektor menggambarkan panjang atau ukuran vektor tersebut. Ada beberapa jenis norma, dengan norma paling umum adalah:

### Norma-2 (Euclidean Norm)

Didefinisikan sebagai:

`||v||₂ = √(Σ(i=1 to n) vᵢ²) = √(v₁² + v₂² + ⋯ + vₙ²)`

**Contoh:**
```
v = [3]
    [4]

||v||₂ = √(3² + 4²) = √(9 + 16) = √25 = 5
```

### Norma-1

Didefinisikan sebagai:

`||v||₁ = Σ(i=1 to n) |vᵢ|`

**Contoh:**
```
v = [-3]
    [ 4]
    [-1]

||v||₁ = |-3| + |4| + |-1| = 3 + 4 + 1 = 8
```

### Norma Tak Hingga (Max Norm)

Didefinisikan sebagai:

`||v||∞ = max(|v₁|, |v₂|, …, |vₙ|)`

**Contoh:**
```
v = [-3]
    [ 4]
    [-1]

||v||∞ = max(|-3|, |4|, |-1|) = max(3, 4, 1) = 4
```

## Aplikasi dalam Machine Learning

### Representasi Data

Dalam Machine Learning, data sering direpresentasikan sebagai vektor. Misalnya, dalam kasus pengenalan gambar, setiap piksel dalam gambar dapat menjadi elemen dari vektor. Jika kita memiliki gambar 28x28 piksel, maka gambar tersebut dapat direpresentasikan sebagai vektor dengan 784 elemen.

**Contoh:**
Untuk klasifikasi email spam:
```
x = [jumlah_kata_'free'        ]
    [jumlah_kata_'buy'         ]
    [panjang_email            ]
    [jumlah_karakter_kapital  ]
    [⋮                       ]
```

### Parameter Model

Parameter dalam model Machine Learning juga sering disimpan dalam bentuk vektor. Misalnya, dalam model regresi linear:

`y = wᵀx + b`

di mana `w` adalah vektor bobot (weights) dan `b` adalah bias.

## Implementasi Python

Berikut adalah contoh implementasi operasi vektor dan skalar menggunakan Python dan library NumPy:

```python
import numpy as np

# Membuat vektor
v = np.array([1, 2, 3])
u = np.array([4, 5, 6])
s = 5

# Operasi dasar
penjumlahan = v + u  # [5, 7, 9]
pengurangan = v - u  # [-3, -3, -3]
perkalian_skalar = s * v  # [5, 10, 15]
penambahan_skalar = v + s  # [6, 7, 8]

# Dot product
dot_product = np.dot(v, u)  # 32

# Norma vektor
norm_l2 = np.linalg.norm(v)  # 3.74 (akar dari 1^2 + 2^2 + 3^2)
norm_l1 = np.linalg.norm(v, ord=1)  # 6 (|1| + |2| + |3|)
```

## Latihan

### Latihan Dasar

**Latihan 1:** Diberikan:
```
a = [ 2]     b = [-3]
    [-1]         [ 2]
    [ 4]         [ 1]
```

Hitung:
1. `a + b`
2. `a - b`
3. `3a`
4. `a · b`

**Jawaban:**
1. `a + b = [-1]`
            `[ 1]`
            `[ 5]`
2. `a - b = [ 5]`
            `[-3]`
            `[ 3]`
3. `3a = [ 6]`
         `[-3]`
         `[12]`
4. `a · b = (2)(-3) + (-1)(2) + (4)(1) = -6 -2 + 4 = -4`

**Latihan 2:** Hitung norma-2 dari vektor berikut:
```
c = [ 3]
    [ 4]
    [12]
```

**Jawaban:**
`||c||₂ = √(3² + 4² + 12²) = √(9 + 16 + 144) = √169 = 13`

**Latihan 3:** Diberikan vektor:
```
d = [-2]
    [ 5]
    [-3]
```

Hitung norma-1 dan norma tak hingga dari vektor tersebut.

**Jawaban:**
- `||d||₁ = |-2| + |5| + |-3| = 2 + 5 + 3 = 10`
- `||d||∞ = max(|-2|, |5|, |-3|) = max(2, 5, 3) = 5`

### Latihan Menengah

**Latihan 4:** Implementasikan fungsi Python untuk menghitung dot product dua vektor tanpa menggunakan library NumPy:

```python
def dot_product(v1, v2):
    if len(v1) != len(v2):
        raise ValueError("Vektor harus memiliki panjang yang sama")
    
    result = 0
    for i in range(len(v1)):
        result += v1[i] * v2[i]
    return result

# Contoh penggunaan
v1 = [1, 2, 3]
v2 = [4, 5, 6]
print(dot_product(v1, v2))  # Output: 32
```

**Latihan 5:** Dua vektor dikatakan ortogonal jika dot product-nya adalah nol. Buat fungsi Python untuk mengecek apakah dua vektor ortogonal:

```python
def are_orthogonal(v1, v2, tolerance=1e-9):
    dot_product_result = dot_product(v1, v2)
    return abs(dot_product_result) < tolerance

# Contoh: vektor [1, 0] dan [0, 1] adalah ortogonal
v1 = [1, 0]
v2 = [0, 1]
print(are_orthogonal(v1, v2))  # Output: True
```

**Latihan 6:** Diberikan dua vektor dalam 3 dimensi:
```
u = [ 2]     v = [-1]
    [-1]         [ 4]
    [ 3]         [ 2]
```

Hitung cross product `u × v`.

**Jawaban:**
```
u × v = [(-1)(2) - (3)(4)]   [-14]
        [(3)(-1) - (2)(2)] = [ -7]
        [(2)(4) - (-1)(-1)]   [  7]
```

### Latihan Lanjutan

**Latihan 7:** Buat fungsi Python untuk menghitung sudut antara dua vektor menggunakan rumus:

`θ = arccos((u · v) / (||u||₂ · ||v||₂))`

```python
import math

def angle_between_vectors(v1, v2):
    dot_prod = dot_product(v1, v2)
    norm_v1 = math.sqrt(sum(x**2 for x in v1))
    norm_v2 = math.sqrt(sum(x**2 for x in v2))
    
    cos_theta = dot_prod / (norm_v1 * norm_v2)
    # Menghindari error karena floating point precision
    cos_theta = max(-1, min(1, cos_theta))
    
    theta_radians = math.acos(cos_theta)
    theta_degrees = math.degrees(theta_radians)
    
    return theta_radians, theta_degrees

# Contoh penggunaan
v1 = [1, 0]
v2 = [0, 1]
radians, degrees = angle_between_vectors(v1, v2)
print(f"Sudut dalam radian: {radians:.4f}")
print(f"Sudut dalam derajat: {degrees:.4f}")  # Output: 90 derajat
```

**Latihan 8:** Dalam Machine Learning, seringkali kita ingin menormalisasi vektor agar memiliki norma-2 sebesar 1. Implementasikan fungsi untuk normalisasi vektor:

```python
def normalize_vector(v):
    norm = math.sqrt(sum(x**2 for x in v))
    if norm == 0:
        raise ValueError("Tidak bisa menormalisasi vektor nol")
    
    return [x / norm for x in v]

# Contoh penggunaan
v = [3, 4]
normalized_v = normalize_vector(v)
print(normalized_v)  # Output: [0.6, 0.8]
# Cek norma: sqrt(0.6^2 + 0.8^2) = sqrt(0.36 + 0.64) = sqrt(1) = 1
```

**Latihan 9:** Dalam konteks Machine Learning, kita sering menggunakan *cosine similarity* untuk mengukur kesamaan antara dua vektor:
`cosine_similarity = (u · v) / (||u||₂ · ||v||₂)`

Implementasikan fungsi untuk menghitung cosine similarity.

```python
def cosine_similarity(v1, v2):
    dot_prod = dot_product(v1, v2)
    norm_v1 = math.sqrt(sum(x**2 for x in v1))
    norm_v2 = math.sqrt(sum(x**2 for x in v2))
    
    if norm_v1 == 0 or norm_v2 == 0:
        return 0  # Jika salah satu vektor adalah vektor nol
    
    return dot_prod / (norm_v1 * norm_v2)

# Contoh penggunaan
v1 = [1, 2, 3]
v2 = [4, 5, 6]
sim = cosine_similarity(v1, v2)
print(f"Cosine similarity: {sim:.4f}")
```

## Kesimpulan

Dalam dokumen ini kita telah membahas:
- Definisi skalar dan vektor
- Representasi matematis dari vektor
- Operasi dasar pada vektor dan skalar (penjumlahan, pengurangan, perkalian)
- Jenis-jenis norma vektor
- Aplikasi vektor dalam Machine Learning
- Implementasi Python untuk operasi vektor
- Latihan-latihan untuk memperkuat pemahaman

Vektor dan skalar merupakan konsep dasar yang sangat penting dalam aljabar linear dan Machine Learning. Pemahaman yang kuat tentang konsep-konsep ini akan sangat membantu dalam memahami topik-topik yang lebih lanjut seperti matriks, transformasi linear, dan algoritma Machine Learning.