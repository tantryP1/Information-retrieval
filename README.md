

---

# Information Retrieval – Sentiment Analysis Twitter

Repositori ini berisi proyek kompetisi dari mata kuliah **Information Retrieval**.
Pada tugas ini, digunakan data komentar Twitter untuk melakukan **klasifikasi sentimen** ke dalam beberapa kategori emosi. Sentimen di sini diartikan sebagai pendapat atau pandangan yang didasarkan pada perasaan terhadap suatu hal.

---

##  Latar Belakang (Overview)

Dalam kompetisi ini, mahasiswa ditantang untuk membangun model pembelajaran mesin yang mampu melakukan klasifikasi terhadap data yang disediakan. Dataset terdiri dari **40.000 sampel** dengan berbagai fitur yang merepresentasikan karakteristik setiap entri.

Tugas utama peserta adalah:

 Memprediksi label kelas pada data uji (**test set**)
 Berdasarkan pola yang dipelajari dari data latih (**training set**)

dengan akurasi setinggi mungkin.

---

##  Hasil Analisis Sentimen Twitter

Laporan ini mencakup tahapan berikut:

* Preprocessing data
* Ekstraksi fitur **TF-IDF (word-level & char-level)**
* Pelatihan model **Logistic Regression**
* Evaluasi performa model
* Visualisasi dataset & hasil prediksi

---

### 🔹 1. Performa Model

| Metrik                     | Nilai                                         |
| -------------------------- | --------------------------------------------- |
| **F1-Score (Macro)**       | **0.2118**                                    |
| **Hyperparameter terbaik** | `{ penalty: l2, solver: liblinear, C: 0.25 }` |

---

### 🔹 2. Ekstraksi Fitur TF-IDF

| Jenis Fitur            | Jumlah     |
| ---------------------- | ---------- |
| Word-level TF-IDF      | 11.628     |
| Character-level TF-IDF | 30.000     |
| **Total fitur**        | **49.404** |

---

### 🔹 3. Informasi Dataset

| Dataset    | Jumlah Sampel |
| ---------- | ------------- |
| Train      | 25.760        |
| Validation | 2.240         |
| Test       | 12.000        |

---

##  4. Visualisasi Dataset

### 4.1 Distribusi Label Sentimen

![Distribusi Label](https://github.com/user-attachments/assets/51cf3013-03f7-4aee-b9a3-b743ec37ad5b)

### 4.2 Distribusi Panjang Tweet

![Distribusi Panjang Tweet](https://github.com/user-attachments/assets/78aa3dbe-b1a3-4fe1-9ba8-b4d335e32172)

---

##  5. Evaluasi Model

### 5.1 Confusion Matrix

![Confusion Matrix](https://github.com/user-attachments/assets/ce3dc1fe-fb01-4ded-b9ae-856020dff82a)

### 5.2 F1-Score per Kelas

![F1 Score](https://github.com/user-attachments/assets/d6c8886a-e1e4-4dad-b3a8-460067ad3095)

---

## 6. WordCloud Setiap Kelas

 Menampilkan kata-kata yang paling dominan pada setiap kelas emosi

Kelas anger
 
Kelas boredom
 
Kelas empty
 
Kelas enthusiasm
 
Kelas fun
 
Kelas happiness
 
Kelas hate
 
Kelas love
 
Kelas neutral
 
Kelas relief
 
Kelas sadness
 
Kelas surprise
 
Kelas worry
 

---

##  7. Kata Paling Berpengaruh (TF-IDF)

Menampilkan **top positive & negative feature weights** untuk setiap kelas emosi.

Disusun per kelas
 Dipisahkan menjadi **Positive Weights** & **Negative Weights**

Kelas anger
Positive weights: begin, pack, zzl, fuckin, fuckin, sheesh, pack, sheesh, jeez, guilti, thinking, aa, throat, rig, aa
Negative weights: hope, still, sad, miss, twitter, new, sleep, still, sad, twitter, week, night, hope, new, love
Kelas boredom
Positive weights: document, tube, minut, hell, one hour, tire, home sick, tube, think make, know today, hell, stuck, boo, bore, bore
Negative weights: lol, see, well, sad, lol, good, good, see, sad, well, back, got, noth, tomorrow, nice
Kelas empty
Positive weights: labor, chang, tri sleep, daddi, optim, labor, le, wardrob, le, dont, bor, wee, wee, bore, bore
Negative weights: miss, love, sad, love, miss, wish, sad, sick, wish, e s, guy, sick, use, good, come
Kelas enthusiasm
Positive weights: get back, interest, someday, releas, nyc, theatr, food, hope, hey, insid, dress, hey, ok, want, want
Negative weights: sad, hate, sorri, sad, hate, job, sorri, hurt, ugh, feel, that, job, lost, hurt, song
Kelas fun
Positive weights: amaz, song, !! , play, haha, play, lol, funni, hah, haha, aha, fun, fun, lol, lol
Negative weights: sad, sad, hate, sorri, hate, miss, hurt, rain, feel, cri, lost, sorri, love, ok, sick
Kelas happiness
Positive weights: glad, haha, excit, enjoy, fun, great, thank, happi, nice, excit, yay, yay, good, happi, great



---

## Kesimpulan Singkat

* Model menggunakan **Logistic Regression + TF-IDF**
* Hasil **macro F1 = 0.2118**
* Tantangan terbesar adalah:

  * banyaknya kelas emosi
  * data tidak seimbang
  * noise pada teks Twitter

