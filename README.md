# Klasifikasi Rambu-Rambu lalu lintas dengan menggunakan python & keras dengan CNN ( Convolutional Neural Network )

## Deskripsi

Proyek "Klasifikasi Rambu Lalu Lintas" memperkenalkan pendekatan inovatif untuk meningkatkan keselamatan jalan dan manajemen lalu lintas melalui penerapan Convolutional Neural Networks (CNN). Seiring dengan pertumbuhan lalu lintas kendaraan yang terus meningkat secara eksponensial, pengenalan rambu lalu lintas yang akurat dan real-time menjadi sangat penting untuk mencegah kecelakaan dan memastikan kelancaran arus lalu lintas. Dengan memanfaatkan kekuatan CNN, kami telah mengembangkan sistem pengenalan rambu lalu lintas yang tangguh dan efisien, yang mampu mengidentifikasi dan mengklasifikasikan berbagai macam rambu lalu lintas yang umum ditemukan di jalan raya.

## Dataset dan Preprocessing Data

Selama proyek ini, kami mengumpulkan dan melakukan pra-pemrosesan pada dataset gambar rambu lalu lintas yang komprehensif, yang mencakup berbagai variasi dalam kondisi pencahayaan, skenario cuaca, dan oklusi (objek yang menghalangi). Persiapan dataset ini memastikan bahwa model kami dapat menangani tantangan di dunia nyata dan memberikan hasil yang andal.

## Model Arsitektur

Inti dari proyek kami adalah model Convolutional Neural Network yang dirancang khusus untuk klasifikasi rambu lalu lintas. Arsitektur modelnya adalah sebagai berikut:

- **Convolutional Layer 1:** 60 filter berukuran (5,5) dengan aktivasi ReLU
- **Convolutional Layer 2:** 60 filter berukuran (5,5) dengan aktivasi ReLU
- **Max Pooling Layer:** Ukuran Pooling (2,2)
- **Convolutional Layer 3:** 15 filter berukuran (3,3) dengan aktivasi ReLU
- **Max Pooling Layer:** Ukuran Pooling (2,2)
- **Dropout Layer:** Tingkat Dropout 0,5 untuk mengurangi overfitting
- **Flatten Layer**
- **Dense Layer 1:** 500 unit dengan aktivasi ReLU
- **Dropout Layer:** Tingkat Dropout 0,5
- **Dense Layer 2:** OLayer output dengan aktivasi softmax (43)

Model ini dikompilasi menggunakan optimizer Adam dengan learning rate 0.001 dan loss function categorical cross-entropy. Dengan melacak akurasi sebagai metrik performa.

## Performa model

Model CNN kami menunjukkan performa yang luar biasa selama pelatihan:

- Mencapai akurasi 95.40% hanya dalam 9 epochs.
- Mencapai nilai loss yang rendah, yaitu 0.1337.

Akurasi yang tinggi dan loss yang rendah ini menunjukkan efektivitas model dalam mengidentifikasi dan mengklasifikasikan rambu lalu lintas secara akurat.
