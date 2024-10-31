# 🐟 İzmir Süpermarket Deniz Ürünleri Sınıflandırma Projesi

Bu proje, İzmir'deki bir süpermarketten toplanan görüntülerle farklı deniz ürünlerini sınıflandırmayı hedefliyor. İzmir Ekonomi Üniversitesi ve bir sanayi kuruluşunun ortak çalışmasıyla elde edilen bu veri seti, toplamda 9 farklı deniz ürünü türüne ait görüntüler içeriyor. Sınıflandırma işlemi, **Yapay Sinir Ağları (ANN)** kullanılarak gerçekleştiriliyor. Bu, özelleşmiş görüntü işleme CNN (Convolutional Neural Network) yapıları olmadan, doğrudan ANN ile balık türlerinin doğru şekilde sınıflandırılmasını hedefleyen yenilikçi bir proje!

## 🗂️ Veri Seti Bilgileri
Veri setinde aşağıdaki balık türlerine ait görüntüler yer almaktadır:
- Gilt Head Bream
- Red Sea Bream
- Sea Bass
- Red Mullet
- Horse Mackerel
- Black Sea Sprat
- Striped Red Mullet
- Trout
- Shrimp

Bu çalışma, üniversite-sanayi iş birliği çerçevesinde yapılmış olup **ASYU 2020**'de yayınlanmıştır.

## 🎯 Proje Yaklaşımı
Bu projede, standart CNN yapılarının aksine, yalnızca **Yapay Sinir Ağı (ANN)** ile sınıflandırma işlemi gerçekleştirilmiştir. CNN'lerin aksine ANN kullanarak:

- **Özellik çıkarımı yapılmadan** görüntüler doğrudan sinir ağına verilmiştir.
- Balık türleri ANN tarafından doğrudan sınıflandırılmıştır.
  
### Neden ANN?
ANN ile çalışmak, genellikle görüntü işleme görevleri için yeterli performansı sağlamasa da, bu proje ANN’in sınıflandırmadaki başarısını ölçmek ve alternatif bir yaklaşım olarak nasıl performans gösterdiğini görmek için önemli bir fırsat sunmaktadır.

## 📈 Proje Amacı ve Kullanılan Teknikler
Projenin nihai amacı, ANN yapısını kullanarak balık türlerini doğru bir şekilde sınıflandırmak ve modelin **genelleme kabiliyetini** artırmaktır. Modelin bilinmeyen verilerde başarısını artırmak adına şu teknikler kullanılmıştır:

- **Early Stopping**: Modelin aşırı öğrenmesini önlemek için belirli bir başarıdan sonra eğitimi durdurur.
- **Dropout**: Aşırı öğrenmeyi engellemek için bazı bağlantıları rastgele iptal ederek modelin daha genel hale gelmesini sağlar.
- **Hiperparametre Optimizasyonu**: Modelin başarımını en üst düzeye çıkarmak için farklı öğrenme oranları, epoch sayıları ve katman yapıları denenmiştir.

## 📊 Çıktılar
1. **Başarım**: Eğitim ve test verileri üzerinde ANN'in doğruluk ve başarı oranları hesaplanmıştır.
2. **J(w) Grafiği**: Her epoch boyunca maliyet fonksiyonundaki azalmayı gösteren grafik çizilmiştir.
3. **Veri Görselleştirmesi**: Eğitim ve test verileri ile model tahmin çizgisi aynı grafikte gösterilerek modelin performansı değerlendirilmiştir.

## 🚀 Nasıl Çalıştırılır
Projeyi çalıştırmak için:
1. `train.txt` ve `test.txt` dosyalarını aynı dizine yerleştirin.
2. İlgili python dosyasını çalıştırarak modeli eğitin ve sonuçları inceleyin.

Görsel veri sınıflandırmada ANN ile elde edilen bu yaklaşım, CNN’lerin olmadığı durumlarda alternatif bir çözüm sunmaktadır.
