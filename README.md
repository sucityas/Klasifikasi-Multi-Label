# Klasifikasi-Multi-Label

Mengklasifikasikan judul buku kedalam jurusan yang sesuai. Model ini dibangun menggunakan metode SEMMA for Data Mining dengan menggunakan Algoritma KNN dan cosine similarity.
Sesuai dengan metode yang digunakan, tahap pembangunan model ini meliputi:
1. Sample
2. Explore
3. Modify
4. Model
5. Asses

# Sample
Sample yang digunakan diambil dari database perpustakaan secara langsung dengan total 20.000 data. Dilakukan cleaning data sehingga didapat 1.223 data bersih. Selanjutnya label yang berbentuk string akan dilakukan binarization dan diubah menjadi label biner sesuai dengan ketentuan klasifikasi multi label.
![image](https://github.com/user-attachments/assets/05a1c00f-3980-4e43-874f-f3fb042ae00d)
Proses Binarization
![image](https://github.com/user-attachments/assets/7ad563f6-0ad2-4ce4-8279-faec873fadb9)

# Explore
Dilakukan eksplorasi pada data agar meminimalisir noise yang akan mempengaruhi kinerja model.
![image](https://github.com/user-attachments/assets/4287550a-b9ea-410a-8977-8e306d94a27d)

# Modify
Dilakukan pre-processing yang terdiri dari case folding, remove numbers, remove punctuation, tokenizing, remove stopwords, dan stemming. Selanjutnya dilakukan pembagian data atau dikenal sebagai splitting data. Kemudian data akan dilakukan pembobotan menggunakan TF-IDF. 
![image](https://github.com/user-attachments/assets/b7a52be4-7c25-4051-9feb-18946628a24e)

# Model
Dalam proses pemodelan, diadopsi algoritma K-Nearest Neighbor dengan metric Cosine Similarity sebagai landasan untuk membangun model serta tambahan metode Grid Search CV dengan harapan kinerja model akan lebih optimal.
![image](https://github.com/user-attachments/assets/530a2152-1c7d-4fa2-a3c0-b04908e5ad81)

# Asses
Menilai tingkat akurasi terhadap algoritma dengan beberapa skenario.
![image](https://github.com/user-attachments/assets/ad410bb4-8e43-4a52-8831-8c7284255e7a)
![image](https://github.com/user-attachments/assets/92ee3df0-7256-492a-82fb-541404357b5e)


