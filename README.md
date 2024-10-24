# AKBANK-10MILIONAI

**### Veri Sınıflandırma Projesi**
Bu proje, görüntü verilerini kullanarak bir yapay zeka modeli oluşturmayı ve modelin performansını artırmayı hedeflemektedir. TensorFlow ve Keras kütüphanelerini kullanarak derin öğrenme yöntemleri ile gerçekleştirilmiştir.

**Kullanılan Teknolojiler**

- Python
- TensorFlow
- Keras
- NumPy
- scikit-learn
- Matplotlib
- Seaborn
- Veri Seti

> Proje, 18 farklı sınıfa ait görüntüler içeren bir veri seti ile çalışmaktadır. Veri setinin boyutları:

- Eğitim verileri: 14,400 görüntü
- Doğrulama verileri: 1,800 görüntü
- Test verileri: 1,800 görüntü



**> Model Yapısı**

> Model aşağıdaki katmanlardan oluşmaktadır:

Giriş Katmanı: 512 nöron, ReLU aktivasyon fonksiyonu.
Gizli Katmanlar: 2 adet gizli katman, her biri 256 nöron.
Çıkış Katmanı: 18 nöron, softmax aktivasyon fonksiyonu.
Model Eğitimi

> Model, 20 epoch boyunca eğitim verileri ile eğitilmiş ve performansı değerlendirilmiştir.

Sınıflandırma raporu, modelinizin her bir sınıf için performansını detaylı bir şekilde sunar. Raporun anlamını ve yorumlanmasını aşağıda bulabilirsiniz:

**Sınıflandırma Raporu**

              precision    recall  f1-score   support

           0       0.91      0.97      0.94       101
           1       0.45      0.54      0.49       107
           2       0.96      0.84      0.89       106
           3       0.64      0.64      0.64        85
           4       0.64      1.00      0.78        95
           5       0.61      0.66      0.63       102
           6       0.99      0.62      0.76       107
           7       0.72      0.34      0.46       105
           8       0.94      0.87      0.91        94
           9       0.78      0.48      0.59        96
          10       0.84      0.83      0.83       111
          11       0.45      0.53      0.49        85
          12       0.84      0.97      0.90       108
          13       0.69      0.72      0.71       101
          14       0.89      0.74      0.81       100
          15       0.46      0.40      0.43        87
          16       0.80      0.85      0.82       93
          17       0.52      0.75      0.62       117

    accuracy                                          0.71      1800
macro avg            0.73          0.71      0.71        1800
weighted avg       0.73          0.71      0.71        1800


### Raporun Bileşenleri

> Precision (Kesinlik):

 Bu değer, modelin doğru pozitif tahminlerinin, toplam pozitif tahminlerine oranıdır. Precision yüksek olduğunda, modelin yanlış pozitif tahminlerde daha az hata yaptığını gösterir.

> Recall (Duyarlılık):
 Modelin gerçek pozitif sınıflarını ne kadar doğru tahmin ettiğini gösterir. Recall yüksek olduğunda, model o sınıfı iyi bir şekilde tanımlıyor demektir.

F1-Score: Precision ve Recall arasında bir denge kuran bir metriktir. 1'e yakın olduğunda, modelin o sınıfta oldukça iyi performans gösterdiğini anlarız.

Support: Her bir sınıf için elimdeki test setinde kaç gözlem olduğunu belirtir.

### Genel Değerlendirme
Doğruluk (Accuracy): Modelin test veri setinde %71 doğruluk elde ettim. Bu, toplam test verisinin %71'inde doğru sınıflandırma yaptığı anlamına geliyor.

Makro Ortalama ve Ağırlıklı Ortalama: Makro ortalama, her sınıfa eşit ağırlık verirken, ağırlıklı ortalama her sınıfın destek (support) sayısına göre ağırlıklandırılmıştır. İkisi de genel performansı değerlendirmek için faydalıdır ve her iki durumda da %71'e yakın sonuç elde ettim.

### Sınıf Bazında Performans
Bazı sınıflarda (örneğin, sınıf 0 ve 2) oldukça yüksek precision ve recall değerleri elde ederken, bazı sınıflarda (örneğin, sınıf 1 ve 15) bu değerler daha düşüktü. Bu da modelin belirli sınıfları daha iyi ayırt edebildiğini, bazı sınıflarda ise daha fazla zorlandığını gösteriyor.

Bu sonuçları göz önünde bulundurarak, model performansını artırmak için daha fazla veri ile eğitmek, hiperparametre optimizasyonu yapmak veya veri artırma yöntemlerini kullanmak gibi iyileştirme yolları izleyebilirim.

Kaggle notebook link: 
[https://www.kaggle.com/code/burcuorhan19/akbank-derin-renme-bootcamp](url)
 

