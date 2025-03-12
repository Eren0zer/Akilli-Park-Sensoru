# 📌 Akıllı Park Sensörü - Öneri Raporu

## 1️⃣ Proje Konusu
Bu proje, ultrasonik sensör ile aracın mesafesini ölçerek sürücüye LED’ler ve sesli uyarılarla geri bildirim sağlayan IoT destekli bir akıllı park sensörü sistemidir. Ölçülen mesafe MQTT protokolü ile bir mobil uygulama veya web paneline gerçek zamanlı olarak gönderilir.

## 2️⃣ Proje Hedefleri
- **Gerçek Zamanlı Mesafe Ölçümü:** Ultrasonik sensör ile doğru mesafe tespiti.
- **Sesli ve Görsel Uyarılar:** LED göstergeler ve buzzer ile sürücüye bildirim sağlamak.
- **IoT Desteği:** MQTT üzerinden uzaktan erişim sağlamak.
- **Güvenli Park:** Kullanıcıya anlık bildirimler ile hatasız park imkanı sağlamak.

## 3️⃣ Tahmini Zaman Çizelgesi
| Görev | Süre (Gün) |
|-------|-----------|
| Proje Planlaması ve Araştırma | 7 |
| Devre Tasarımı ve Donanım Montajı | 10 |
| Yazılım Geliştirme (ESP32 Kodlama) | 14 |
| IoT Entegrasyonu ve MQTT Testleri | 10 |
| Test ve Hata Giderme | 10 |
| Raporlama ve Sunum Hazırlığı | 5 |
| **Toplam Süre** | **56 Gün** |

## 4️⃣ Kaynak Planlaması
- **Ekip Üyeleri:**
  - Elektronik Mühendisi: Devre tasarımı ve montaj.              ->  İlhan Emre Adak, Eren Özer  
  - Yazılım Geliştirici: ESP32 programlama ve MQTT entegrasyonu. ->  Sıdıka Firat, Şevval Yavuz
  - Proje Yöneticisi: Takım koordinasyonu ve dokümantasyon.      ->  Eren Özer

### 📋 Maliyet ve Ekipmanlar

| Malzeme                          | Miktar  | Fiyat (₺)  |
|----------------------------------|---------|------------|
| ESP32 veya ESP8266               | 1       | 270        |
| HC-SR04 Ultrasonik Sensör        | 1       | 50         |
| LED (Kırmızı/Sarı/Yeşil)         | 5       | 10         |
| Buzzer                           | 1       | 10         |
| Dirençler                        | Çeşitli | 5          |
| Breadboard ve Jumper Kabloları   | 1 Set   | 60         |
| **Toplam Tahmini Maliyet**       | **-**   | **405₺**   |


## 5️⃣ Risk Analizi
| Risk Faktörü | Olasılık | Etki | Çözüm Önerisi |
|-------------|---------|------|----------------|
| Sensör Yanlış Okuma | Orta | Yüksek | Kalibrasyon ve kod optimizasyonu yapılmalı. |
| MQTT Bağlantı Kopmaları | Yüksek | Orta | Stabil bir MQTT broker kullanılmalı ve bağlantı tekrar denemeleri eklenmeli. |
| Kullanıcı Arayüzü Sorunları | Orta | Orta | Kullanıcı testleri ile optimize edilmeli. |
| Donanım Arızası | Düşük | Yüksek | Yedek malzeme bulundurulmalı. |

## 6️⃣ Ticari Potansiyel
- **Otomotiv Endüstrisi:** Fabrika çıkışlı araçlarda akıllı park sistemleri.
- **Araç Modifikasyon Pazarı:** Eski model araçlar için ek park sensörü.
- **Akıllı Şehir Projeleri:** Trafik akışını optimize etmek için veri toplayan sistemler.
- **Otopark Yönetimi:** Araç park alanlarını optimize eden sistemlere entegrasyon.


