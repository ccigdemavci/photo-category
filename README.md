Görüntü Sınıflandırma (CNN) - README
📌 Proje Hakkında
Bu proje, Convolutional Neural Network (CNN) kullanarak 8 farklı görüntü sınıfını tanıyan bir görüntü sınıflandırma modelini içermektedir. Görseller /goru2 adlı bir klasörde organize edilmiştir. Model, TensorFlow/Keras kullanılarak sıfırdan oluşturulmuş ve eğitim sürecinde veri artırımı, erken durdurma gibi tekniklerle optimize edilmiştir.

🧠 Kullanılan Teknolojiler
Python 3

TensorFlow / Keras

NumPy

Matplotlib

scikit-learn

📂 Veri Seti Yapısı
Veri seti, 8 farklı sınıfa ait görüntülerin bulunduğu alt klasörlerden oluşur. Aşağıdaki gibi bir dizin yapısı beklenir:

bash
Kopyala
Düzenle
/goru2
│
├── sinif1/
│   ├── img1.jpg
│   ├── img2.jpg
│   └── ...
├── sinif2/
│   └── ...
├── ...
└── sinif8/
🚀 Model Mimarisi
Model aşağıdaki CNN yapısını kullanır:

4 adet Conv2D + MaxPooling2D bloğu

1 adet Flatten katmanı

1 adet Dense (512) katmanı

Softmax çıkış katmanı (sınıf sayısı kadar nöron içerir)

🏋️‍♀️ Eğitim Süreci


Görsel boyutu: 150x150

Batch boyutu: 32

Epoch: 10

Loss: categorical_crossentropy

Optimizasyon: adam

Validation Split: %20

EarlyStopping: patience=5

📈 Sonuçlar
Modelin eğitimden sonra başarı oranı ve hata oranları:


❌ Eğitim Hata Oranı: 0.0471

❌ Doğrulama Hata Oranı: 0.1591



📌 Notlar
Daha yüksek doğruluk için:

Epoch sayısı artırılabilir.

Veri sayısı dengelenebilir.

Daha karmaşık modeller (ör. MobileNetV2) transfer learning ile entegre edilebilir.

early_stopping aktif olduğundan model aşırı öğrenmeden korunmuştur.

👩‍💻 Geliştirici
Cigdem Avci - Bilgisayar Mühendisliği Öğrencisi
GitHub: github.com/cigdemavci
Proje: Görüntü Sınıflandırma ve CNN Eğitimi



Youtube:  https://www.youtube.com/watch?v=VhHDebgRRDg
