# 🧠 BraTS 2020 - MRI Veri Hazırlama (Preprocessing Pipeline)

Bu proje, **BraTS 2020** beyin tümörü veriseti ile çalışmak üzere geliştirilmiş bir **veri ön işleme** ve eğitim öncesi hazırlık pipeline'ıdır.

> ✨ Proje Sahibi: **Rukiye İlhan**
> 📚 Amaç: Beyin MR görüntülerini derin öğrenme modellerine hazır hale getirmek

---

## 🎯 Proje Amacı

* NIfTI (.nii.gz) formatındaki beyin MR görüntülerini yüklemek
* Verileri normalize etmek, yeniden boyutlandırmak ve .npy formatına dönüştürmek
* Eğitim/validasyon/test ayrımı yapmak
* (Devamında) TensorFlow tabanlı modellerle eğitim gerçekleştirmek


---

## 🧰 Kullanılan Kütüphaneler (Detaylı)

| Kategori                           | Kütüphane                              | Açıklama                                                                                                 |
| ---------------------------------- | -------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| **🧠 Medikal Görüntüleme (NIfTI)** | `nibabel`                              | NIfTI (.nii.gz) formatındaki beyin MR görüntülerini okumak ve yazmak için kullanılır.                    |
| **🔢 Sayısal Hesaplama**           | `numpy`                                | Çok boyutlu diziler ve matrisler üzerinde hızlı işlemler yapılmasını sağlar.                             |
| **📊 Görselleştirme**              | `matplotlib.pyplot`                    | Görüntüleri, histogramları veya eğitim sürecini görselleştirmek için kullanılır.                         |
| **🗂️ Dosya/Dizin Yönetimi**       | `os`, `glob`, `shutil`, `splitfolders` | Dosya yolları, klasör ayrımı, eğitim/validasyon/test klasörlerinin oluşturulması ve taşınması işlemleri. |
| **⚙️ Görüntü/Sinyal İşleme**       | `scipy.signal`                         | Medikal veriler üzerinde filtreleme ve ileri sinyal işleme adımları (opsiyonel) için kullanılır.         |
| **🎲 Rastgelelik / Veri Dağılımı** | `random`                               | Veri karıştırma veya örnek seçimi gibi işlemlerde rastgelelik sağlar.                                    |
| **🧪 Önişleme / Normalize**        | `sklearn.preprocessing.MinMaxScaler`   | Görüntü verilerini 0–1 aralığına normalize eder. Özellikle model eğitimi öncesinde önemlidir.            |
| **🧠 Derin Öğrenme ve Modelleme**  | `tensorflow.keras`, `tensorflow`       | Katman oluşturma, eğitim, callback, optimizasyon gibi tüm modelleme süreci burada yapılır.               |

---

## 🔄 Devam Eden Aşamalar

Bu proje hâlen geliştirme aşamasındadır. Aşağıdaki adımlar tamamlanacaktır:

* [x] Veri yükleme ve düzenleme
* [x] Normalize etme ve `.npy` formatına çevirme
* [x] Eğitim/validasyon/test ayrımı
* [ ] Model mimarisinin tanımlanması
* [ ] Model eğitimi ve performans analizi
* [ ] Segmentasyon çıktılarının görselleştirilmesi

---

## 👩‍💻 Geliştirici Bilgisi

**Rukiye İlhan**
Bilgisayar Mühendisliği Öğrencisi
Yapay zeka, görüntü işleme ve sağlıkta derin öğrenme alanlarına ilgi duymaktadır.

📫 İletişim: `ilhanxrukiye@gmail.com`

---

## 📜 Lisans ve Kullanım

BraTS2020 veriseti, Medical Segmentation Decathlon kapsamında sunulmuş açık bir veri kaynağıdır. Bu proje eğitim ve araştırma amaçlı hazırlanmıştır.
