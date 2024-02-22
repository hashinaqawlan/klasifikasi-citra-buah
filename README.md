**Klasifikasi Citra Buah Jeruk Segar dan Busuk dengan Convolutional Neural Network (CNN)**


Dalam kehidupan sehari-hari manusia seringkali melakukan proses klasifikasi untuk mempermudah pekerjaan. Banyak hal lebih mudah dilakukan ketika kita dapat mengklasifikasikan dengan memanfaatkan teknologi salah satunya dalam bidang pertanian. Dengan pemanfaatan teknologi ini membuat proses produksi lebih efektif dan efisien salah satunya dalam proses sortir. Pada proses sortir ini biasanya ditetapkan beberapa kriteria hasil panen, seperti dari ukuran, bentuk, warna dan kualitasnya. Jika proses klasifikasi bisa dilakukan dengan tepat dan cepat, maka hal ini dapat membantu petani dalam meningkatkan hasil produksi dan mampu bersaing di pasaran. Maka dari itu dalam penelitian ini dilakukan proses klasifikasi dengan mendeteksi buah jeruk segar dan buah jeruk busuk.

Data yang peneliti gunakan adalah data citra berupa gambar buah jeruk dengan klasifikasi jeruk busuk dan jeruk segar. Dalam hal ini peneliti menggunakan metode jaringan syaraf tiruan atau Convolutional Neural Network (CNN). 

![gambar arsitektur](https://github.com/hashinaqawlan/klasifikasi-citra-buah/assets/104309456/693fb0d6-af0d-4b88-9b63-f56762e5d971)

Arsitektur CNN dalam penelitian ini memiliki 3 lapisan konvolusi (convolutional layer) yang menggunakan fungsi aktivasi ReLu dan dipadukan dengan max pooling layer. Pada layer konvolusi yang pertama terdapat 32 feature maps dengan ukuran matriks 3x3. Lalu dilakukan proses pooling menggunakan 2x2. Pada layer konvolusi kedua menggunakan 64 feature maps dan konvolusi ketiga menggunakan 128 feature maps dengan ukuran, fungsi aktivasi dan proses pooling yang sama seperti pada layer konvolusi pertama. 

Proses selanjutnya adalah layer fully connected yang pertama merupakan flatten. Kemudian pada layer dense, masing-masing flatten akan dilewatkan ke 512 neuron. Setelah itu pada layer dense kedua yakni dengan jumlah sebesar jumlah kelas yang akan diklasifikasikan. Pada penelitian ini, layer output menggunakan layer dense sebanyak 1. Fungsi aktivasi yang digunakan pada fully connected layer adalah Softmax.
Penelitian ini melakukan uji akurasi pada proses training dan testing dengan akurasi pada proses training didapatkan sebesar 91,74% dan akurasi pada proses testing menggunakan 560 citra baru didapatkan sebesar 95%.
