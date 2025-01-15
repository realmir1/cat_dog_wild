

# Hayvan Yüzlerini Sınıflandıran Yapay Sinir Ağı 

Bu proje, hayvan yüzlerini sınıflandırmak için evrişimli sinir ağı (CNN) modelini kullanan bir görüntü işleme uygulamasıdır. Model, kedi, köpek ve vahşi hayvan kategorilerinde sınıflandırma yapmaktadır. TensorFlow ve Keras kütüphaneleri kullanılarak geliştirilmiştir ve verilerin işlenmesinden modelin eğitilmesine kadar tüm adımları içermektedir.

---


## **Geliştirildiği Ortamlar**
- Visual Studio Code
- Kaggle
 <br>
<p align ="center">  <img src="https://opendatascience.com/wp-content/uploads/2018/12/kaggle.png" ,width= "500", height="300"</p>




## **Projenin Amacı**  
Bu proje, hayvan yüzlerini otomatik olarak tanıyabilen ve sınıflandırabilen bir model geliştirmeyi hedeflemektedir. Model, aşağıdaki sınıflarda sınıflandırma yapmaktadır:  
- **Kedi (cat)** 🐈   
- **Köpek (dog)**  🐕
- **Vahşi hayvan (wild)** 🐅

Bu tür bir sınıflandırma modeli, örneğin hayvan davranışlarını analiz etmek, doğada hayvan popülasyonlarını izlemek veya benzer görüntü işleme projelerinde kullanılabilir.



## **Veri Kümesi Hakkında**  
Proje, hayvan yüzlerini içeren bir veri kümesi kullanmaktadır. Veri kümesi, her bir hayvan kategorisi için ayrı klasörlere sahip olacak şekilde organize edilmiştir. Verilerin organize edilmesi şu şekildedir:  

```
afhq/
└── train/
    ├── cat/
    ├── dog/
    └── wild/
```


Bu dizin yapısı, modelin veri akışını kolayca sağlayabilmesi için önemlidir. Veri kümesini indirip `/kaggle/input/animal-faces/afhq/train` dizinine yerleştirmeniz gerekmektedir.
<br>
<p align="center">
  <img src="https://cdn.dribbble.com/users/668001/screenshots/3861883/data-graphic-animation.gif" alt="Example GIF" height="300", width="400">
</p>

 ## **Modelin Eğitilmesi**  
   Model, 10 epoch boyunca `adam` optimizasyon algoritması kullanılarak eğitilmiştir. Kategorik çapraz entropi kaybı (`categorical_crossentropy`) kullanılmış ve doğruluk (`accuracy`) metriği takip edilmiştir.
<br>
<p align="center">
  <img src="https://static.wixstatic.com/media/0046d0_40f27fb5dc434ffa8e86ec0bb1444c1b~mv2.gif" alt="Example GIF" height="300", width="400">
</p>

 ## **Performans Analizi**  
   Eğitim sırasında elde edilen doğruluk ve doğrulama verileri matplotlib kullanılarak grafiklerle görselleştirilmiştir. Bu sayede modelin performansı detaylı bir şekilde analiz edilmiştir.
<br>
<p align="center">
  <img src="https://i.pinimg.com/originals/39/9d/50/399d509c00b8cbfe0c7ddffb3b40a705.gif" alt="Example GIF" height="300", width="400">
</p>

 ## **Tahmin ve Görselleştirme**  
   Model, doğrulama setinden rastgele 10 görüntü için tahminlerde bulunmuştur. Bu tahminler, gerçek etiketlerle karşılaştırılmış ve görüntüler üzerinde görselleştirilmiştir.  
<br>
<p align="center">
  <img src="https://miro.medium.com/v2/resize:fit:2400/1*36MELEhgZsPFuzlZvObnxA.gif" alt="Example GIF" height="300", width="400">
</p>



## **Sonuçlar ve Çıktılar**  
- Model, veri kümesindeki hayvan yüzlerini yüksek doğrulukla sınıflandırmayı başarmıştır.  
- Eğitim ve doğrulama sonuçları grafiklerle analiz edilmiştir.  
- Örnek tahminler, modelin sınıflandırma başarısını görselleştirmek için sunulmuştur.  

<p align="center"> <img sr</p>

## **Nasıl Çalıştırılır?**  
1. Proje dosyalarını indirin ve aşağıdaki adımları takip edin:  
   - Veri kümesini `/kaggle/input/animal-faces/afhq/train` dizinine yerleştirin.  
   - Python ortamınızı gerekli kütüphanelerle kurulum yapacak şekilde hazırlayın.  

2. Gerekli kütüphaneleri yüklemek için aşağıdaki komutu çalıştırabilirsiniz:  
   ```
   pip install tensorflow matplotlib numpy
   ```

3. Kod dosyasını çalıştırarak modeli eğitin ve sonuçları gözlemleyin.

---

**Gerekli Kütüphaneler**  
- Python 3.x  
- TensorFlow  
- Keras  
- Matplotlib  
- NumPy  

---

**Kütüphanelerin Kullanıldığı Yerler**

| Kütüphaneler       | Kullanım Alanı       |
|--------------------|----------------------|
| TensorFlow         | Derin Öğrenme        |
| Keras              | Derin Öğrenme        |
| Matlpotlib         | Grafik İşleme        |
| Numpy              | İşleme               | 


## Keras <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/ae/Keras_logo.svg/1200px-Keras_logo.svg.png" width="35" align="left">

Keras, derin öğrenme (deep learning) uygulamaları geliştirmek için kullanılan açık kaynaklı bir Python kütüphanesidir. Başlangıçta Theano ve TensorFlow gibi arka uç kütüphanelerine dayanarak çalışıyordu, ancak günümüzde TensorFlow'un yüksek seviyeli API'si olarak entegre edilmiştir. Keras, kullanıcı dostu ve modüler bir yapıya sahip olup, hızlı prototipleme, eğitim ve derin öğrenme modellerinin geliştirilmesi için idealdir.
<br>
<p align="center">
  <img src="https://miro.medium.com/v2/resize:fit:2400/1*36MELEhgZsPFuzlZvObnxA.gif" alt="Example GIF" height="300", width="400">
</p>

## Numpy <img src="https://numpy.org/images/logo.svg" alt="Numpy Logo" width="35" align="left">
NumPy, Python dilinde büyük sayılar ve çok boyutlu diziler üzerinde hızlı ve etkili matematiksel işlemler gerçekleştirmeye olanak sağlayan bir python kütüphanedir. NumPy, aynı zamanda Python'da matematiksel işlemler yapmak için kullanılan diğer kütüphanelerle uyumlu bir şekilde çalışır.
<br>
<p align="center">
  <img src="https://matteding.github.io/images/broadcasting-3d-scalar.gif" alt="Example GIF" height="300", width="400">
</p>

## Tensorflow <img src="https://avatars.githubusercontent.com/u/15658638?s=280&v=4" alt="Numpy Logo" width="35" align="left">
TensorFlow, makine öğrenimi için ücretsiz ve açık kaynaklı bir yazılım kütüphanesidir . Bir dizi görevde kullanılabilir, ancak derin sinir ağlarının eğitimi ve çıkarımına özel olarak odaklanmaktadır
<br>
<p align="center">
  <img src="https://www.tensorflow.org/static/site-assets/images/marketing/cards/spotify-tensorflow-agents-recommendation-systems.gif" alt="Example GIF" height="300", width="400">
</p>

## Matplotlib <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/01/Created_with_Matplotlib-logo.svg/2048px-Created_with_Matplotlib-logo.svg.png" alt="Numpy Logo" width="35" align="left">
Matplotlib, Python programlama dilinin temel çizim kitaplığıdır. Python görselleştirme paketleri arasında en yaygın kullanılanıdır.

<br>
<p align="center">
  <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEg2ZvFv81XgsfhwqoAM0MOKKtzuVfhxw77xDMFd33AzpZ0ErQLp0e53PNItYnE7cbZuLYd4Ssv2CG540RE1h1nUS3PU5jLF71Zg-jYaxI5mFZXVSvZnnklptUxR3bd2VP28it24tt8op9QH/s400/plot_surface_animation_funcanimation_r.gif" height="300", width="400">
</p>

## **Kullanım Alanları**  
Bu proje, hayvan sınıflandırmasının ötesinde şu gibi uygulama alanlarına uyarlanabilir:  
- Vahşi yaşam araştırmaları  
- Görüntü tabanlı hayvan davranışı analizleri  
- Hayvanların popülasyonlarını otomatik takip sistemleri  

---





