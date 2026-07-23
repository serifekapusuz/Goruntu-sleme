# Görüntü İşleme Karşılaştırma Aracı: OpenCV vs Manuel

Bu proje, popüler görüntü işleme kütüphanesi OpenCV'nin sunduğu hazır fonksiyonlar ile bu algoritmaların NumPy tabanlı (manuel) uygulamalarını eşzamanlı olarak karşılaştıran modern arayüzlü bir masaüstü uygulamasıdır. Öğrenciler, araştırmacılar ve görüntü işlemeye yeni başlayanlar için arka planda çalışan matematiği anlamaya yönelik interaktif bir eğitim aracı olarak tasarlanmıştır.

<img width="1920" height="1140" alt="Ekran görüntüsü 2025-12-18 011111" src="https://github.com/user-attachments/assets/a5e3cd18-b1a8-49f6-9ea9-65f5f613a0c8" />
<img width="1920" height="1140" alt="Ekran görüntüsü 2025-12-18 010951" src="https://github.com/user-attachments/assets/0d56db74-4dba-4e1e-b45f-e7d7fc09f8aa" />

## 🚀 Özellikler

- **Modern ve Karanlık Tema UI:** `customtkinter` kullanılarak geliştirilmiş, kullanıcı dostu şık arayüz.
- **Eşzamanlı Karşılaştırma:** Orijinal resim, OpenCV çıktısı ve Manuel kod çıktısını aynı ekranda yan yana görüntüleme.
- **Dinamik Kod İnceleme:** Seçilen algoritmanın her iki (OpenCV ve Manuel) yaklaşımı için kullanılan gerçek Python kaynak kodlarını anlık olarak ekranda görebilme (`inspect` modülü ile).
- **Gerçek Zamanlı Parametre Kontrolü:** Eşik (threshold), kernel boyutu, açı, kontrast katsayısı gibi değerleri slider (sürgü) ile anında değiştirip sonuçları gözlemleyebilme.
- **Türkçe Karakter Desteği:** Dosya yollarındaki Türkçe karakter sorunları özel okuma yöntemleriyle giderilmiştir.
- **29 Farklı Algoritma:** Temel piksel işlemlerinden, morfolojik filtrelere ve özellik çıkarımına kadar geniş algoritma kütüphanesi.

## 🧰 İçerdiği Algoritmalar

Toplam 29 farklı görüntü işleme işlemi 5 ana kategoride toplanmıştır:

1. **Renk ve Piksel İşlemleri:** Sınırlama (Clipping), Parlaklık, Kontrast, Gri Seviye (Grayscale), Negatif, Binary Thresholding.
2. **Filtreleme (Bulanıklaştırma):** Mean Filter, Gaussian Blur, Median Blur.
3. **Kenar Bulma ve Türev İşlemleri:** Canny Edge Detection, Laplacian, Sobel (X/Y), Prewitt (X/Y).
4. **Geometrik Dönüşümler:** Döndürme (Rotation), Çevirme (Vertical/Horizontal Flip), Kaydırma (Translation), Yakınlaştırma/Uzaklaştırma (Zoom In/Out).
5. **Morfolojik ve İleri Seviye İşlemler:** Erosion, Dilation, Opening, Closing, Open+Close, Histogram Çizimi, Histogram Eşitleme, Özellik Çıkarımı (Harris Corner).

## 🛠️ Kurulum ve Gereksinimler

Projeyi kendi bilgisayarınızda çalıştırmak için sisteminizde Python 3.x yüklü olmalıdır. Gerekli kütüphaneleri kurmak için aşağıdaki komutu terminalinizde (veya komut istemcisine) çalıştırın:

```bash
pip install customtkinter opencv-python numpy pillow matplotlib

