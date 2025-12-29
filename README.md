<img width="729" height="521" alt="image" src="https://github.com/user-attachments/assets/bca07a9f-ef68-4256-9ff1-ed178857b6ae" /># Information-retrieval
Merupkan kompetisi dari mata kuliah infomation retrieval
Dalam tugas ini, kita akan menggunakan data komen twitter untuk mengklasifikasikan atau mengkategorikan data tersebut menjadi beberapa klasifikasi sentimen, dimana sentimen adalah pendapat atau pandangan yg didasarkan pd perasaan yg berlebih-lebihan thd sesuatu.

### Latar Belakang (Overview)

Dalam kompetisi ini, mahasiswa ditantang untuk membangun model pembelajaran mesin yang mampu melakukan klasifikasi terhadap data yang disediakan. Dataset ini berisi 40.000 sampel, dengan berbagai fitur yang mewakili karakteristik dari setiap entri.

Tugas utama peserta adalah memprediksi label kelas dari data uji (test set) seakurat mungkin berdasarkan pola yang dipelajari dari data latih (training set).


### Hasil Dari Percobaan
LAPORAN ANALISIS SENTIMEN TWITTER
Rangkuman lengkap proses analisis sentimen yang meliputi:
-	Preprocessing data
-	Ekstraksi fitur TF-IDF word-level dan char-level
-	Pelatihan model Logistic Regression
-	Evaluasi performa model
-	Visualisasi dataset dan hasil prediksi
1. Performa Model
F1-Score (Macro): 0.2118
Hyperparameter Terbaik: {'penalty': 'l2', 'solver': 'liblinear', 'C': 0.25}
2. Ekstraksi Fitur TF-IDF
Word-level TF-IDF: 11628 fitur
Character-level TF-IDF: 30000 fitur Total Fitur: 49404 fitur
3. Informasi Dataset
Train samples: 25760
Validation samples: 2240 Test samples: 12000
4. Visualisasi Dataset
4.1 Distribusi Label Sentimen
 <img width="729" height="521" alt="image" src="https://github.com/user-attachments/assets/51cf3013-03f7-4aee-b9a3-b743ec37ad5b" />

4.2 Distribusi Panjang Tweet
 <img width="729" height="521" alt="image" src="https://github.com/user-attachments/assets/78aa3dbe-b1a3-4fe1-9ba8-b4d335e32172" />

5. Evaluasi Model
5.1 Confusion Matrix
 <img width="729" height="625" alt="image" src="https://github.com/user-attachments/assets/ce3dc1fe-fb01-4ded-b9ae-856020dff82a" />

5.2 F1-Score per Kelas
 <img width="729" height="521" alt="image" src="https://github.com/user-attachments/assets/d6c8886a-e1e4-4dad-b3a8-460067ad3095" />

6. WordCloud Setiap Kelas
Kelas anger
 <img width="667" height="417" alt="image" src="https://github.com/user-attachments/assets/761ef415-4b9d-46f3-b988-7a78f7be6bd2" />

Kelas boredom
 <img width="667" height="417" alt="image" src="https://github.com/user-attachments/assets/a3485c14-ae47-482f-b632-42c25970a8c8" />

Kelas empty
 <img width="667" height="417" alt="image" src="https://github.com/user-attachments/assets/f418260b-2dee-41b8-ae32-7d67a394c7cb" />

Kelas enthusiasm
 <img width="667" height="417" alt="image" src="https://github.com/user-attachments/assets/318e61a9-55ce-4600-b300-4e224408d459" />

Kelas fun
 <img width="667" height="417" alt="image" src="https://github.com/user-attachments/assets/5e151a4b-ade7-403c-a731-55dd31d3a11a" />

Kelas happiness
<img width="667" height="417" alt="image" src="https://github.com/user-attachments/assets/82dc56c3-731b-4332-99de-43a1160e56a6" />
 
Kelas hate
 <img width="667" height="417" alt="image" src="https://github.com/user-attachments/assets/42961259-f9b7-486a-a1e1-1be69c592de7" />

Kelas love
 <img width="667" height="417" alt="image" src="https://github.com/user-attachments/assets/a6506ffc-9199-45c7-9dc8-38f69a75d9ae" />

Kelas neutral
<img width="667" height="417" alt="image" src="https://github.com/user-attachments/assets/3ddb8a8d-c395-43a3-9dc2-49d787fd92cb" />
 
Kelas relief
 <img width="667" height="417" alt="image" src="https://github.com/user-attachments/assets/6f76f07a-0aee-4183-b7eb-7692eb30a7bb" />

Kelas sadness
 <img width="667" height="417" alt="image" src="https://github.com/user-attachments/assets/36956afc-4b9d-4e58-b2c4-35fdcd4ceb22" />

Kelas surprise
 <img width="667" height="417" alt="image" src="https://github.com/user-attachments/assets/af492223-6a8e-4283-b765-640162f2c2ad" />

Kelas worry
<img width="667" height="417" alt="image" src="https://github.com/user-attachments/assets/ee081f25-07d5-4d5e-878a-184cd5e5fff5" />
 
7. Kata Paling Berpengaruh (TF-IDF)
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
Negative weights: sad, hate, sad, hate, miss, suck, sick, suck, bad, sorri, feel, hurt, ugh, sick, bore
Kelas hate
Positive weights: piss, uck, shit, ass, shit, stupid, ass, damn, stupid, suck, fuck, suck, fuck, hate, hate
Negative weights: miss, love, sad, miss, lol, sad, lol, hope, love, nice, thank, great, wish, fun, good
Kelas love
Positive weights: lt, ove, cute, hug, love, lt, ove , love, cute, lov, love , hug, lov, love, love
Negative weights: sad, sad, tire, bad, work, hurt, tire, bore, live, live, happen, it, sorri, it, hurt
Kelas neutral
Positive weights: number, post, ye, th, link, watch, work, th, link, ork, good night, check, check, nope, nope
Negative weights: sad, love, sad, miss, love, hate, feel, sick, suck, oh, hurt, happi, hate, bad, sick
Kelas relief
Positive weights: thank, school today, worri, thank god, least, fine, done, glad, thank, relax, relax, done, glad, final, final
Negative weights: sad, miss, miss, cant, hate, sad, wish, hate, mean, fuck, good morn, cant, wish, fuck, mean
Kelas sadness
Positive weights: sa, depress, sad, hurt, sadli, sadli, sad, depress, cri, hurt, miss, cri, miss, sad, sad Negative weights: thank, hope, thank, hope, good, haha, may, great, haha, great, good, th, lol, morn, look
Kelas surprise
Positive weights: believ, really, thought, really, what, surpris, what, oh, believ, surpris, oh, omg, omg, wow, wow
Negative weights: feel, miss, hate, feel, miss, today, hate, readi, good, love, love, bore, work, way, us
Kelas worry
Positive weights: pleas, bad, sick, hurt, scare, sorri, find, sick, sorri, hope, feel, hope, poor, poor, feel
Negative weights: thank, love, thank, love, nice, song, new, hate, nice, haha, week, song, hah, haha, great
