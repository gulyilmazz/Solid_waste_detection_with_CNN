# Solid Waste Detection with CNN

Bu proje, farklı atık türlerini (karton, cam, metal, kağıt, plastik, çöp vb.) görüntü tabanlı bir derin öğrenme modeli ile sınıflandırmayı amaçlar. Projede eğitim verisi, eğitim ve değerlendirme kodları ile eğitim sonrası kaydedilmiş bir model (`mymodel.keras`) bulunmaktadır.

Öne çıkan içerikler
- `cnn_kati_atik.ipynb` - Projenin eğitim ve değerlendirme adımlarını içeren Jupyter notebook.
- `mymodel.keras` - Eğitilmiş Keras modeli (inference için kullanılabilir).
- `Garbage_classification/Garbageclassification/` - Etiketlenmiş görüntü veri seti; içinde sınıf klasörleri bulunur (ör. `cardboard`, `glass`, `metal`, `paper`, `plastic`, `trash`).
- `deney1.jpg`, `deney2.jpg` - Hızlı test/deney amaçlı örnek görüntüler.

İçerik ve klasör yapısı (kısaca)

Garbage_classification içinde sınıflara göre ayrılmış resimler bulunur. Tipik yapı:

```
Garbage_classification/
	Garbageclassification/
		cardboard/
		glass/
		metal/
		paper/
		plastic/
		trash/
```

Kurulum (geliştirme ortamı - öneri, PowerShell için)

1) Sanal ortam oluşturun ve etkinleştirin:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

2) Gerekli paketleri yükleyin (örnek paket listesi):

```powershell
pip install tensorflow numpy pillow matplotlib scikit-learn opencv-python
```

Not: Projeye özel bir `requirements.txt` yoksa yukarıdaki paketleri yükleyerek başlamanız yeterlidir. Eğer isterseniz ben sizin için bir `requirements.txt` oluşturabilirim.

Hızlı başlangıç

- Jupyter Notebook ile `cnn_kati_atik.ipynb` dosyasını açarak veri ön işleme, model mimarisi, eğitim ve değerlendirme adımlarını çalıştırabilirsiniz.
- Eğitim tamamlandıktan sonra `mymodel.keras` dosyası ile doğrudan tahmin yapabilirsiniz.


