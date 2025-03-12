# Akıllı Park Sensörü (IoT Destekli Sesli ve Görsel Uyarı Sistemi)

## 📌 Proje Konusu
Bu proje, ultrasonik sensör ile aracın mesafesini ölçerek sürücüye LED’ler ve sesli uyarılarla geri bildirim sağlayan akıllı bir park sensörü sistemidir. IoT desteği ile ölçülen mesafe MQTT üzerinden bir mobil uygulama veya web paneline gerçek zamanlı olarak gönderilir.

## 📡 Proje Kısa Özeti
- Ultrasonik sensör ile aracın mesafesini ölçer.
- 5 adet LED ile görsel uyarı sağlar.
- Buzzer ile sesli uyarı verir.
- MQTT protokolü ile mesafe bilgisi mobil/web uygulamasına iletilir.

## 📋 Proje Gereksinimleri
Bu projeyi çalıştırmak için aşağıdaki malzemelere ve yazılımlara ihtiyaç vardır:

### **Donanım Gereksinimleri:**
| Malzeme | Açıklama |
|---------|---------|
| ESP32 veya ESP8266 | Ana kontrol kartı (Wi-Fi bağlantısı için) |
| HC-SR04 Ultrasonik Sensör | Mesafe ölçümü için |
| 5x LED  | Mesafeye göre park durumu göstergesi |
| Buzzer (Aktif/Pasif) | Sesli uyarı vermek için |
| Dirençler (220Ω) | LED’leri güvenli çalıştırmak için |
| Breadboard ve Jumper Kabloları | Bağlantılar için |
| Wi-Fi Ağı | MQTT bağlantısı için |

### **Yazılım Gereksinimleri:**
- Arduino IDE veya PlatformIO
- MQTT Broker (HiveMQ, Adafruit IO veya Mosquitto)
- ESP32/ESP8266 kütüphaneleri

## 🚀 Projeyi Çalıştırma
1. **Gerekli Kütüphaneleri Yükleme:**
   - Arduino IDE üzerinden aşağıdaki kütüphaneleri yükleyin:
     - `ESP8266WiFi` veya `WiFi` (ESP32 için) // Wi-Fi bağlantısını sağlayan kütüphane
     - `PubSubClient` (MQTT bağlantısı için) // MQTT protokolü üzerinden veri gönderme/alma işlemleri
     - `NewPing` (Ultrasonik sensör için) // Sensör verilerini işlemek için kullanılır

2. **Bağlantıları Yapın:**
   - HC-SR04 sensörünü ESP modülüne bağlayın. // Mesafe ölçümü için kullanılır
   - LED’leri uygun dirençlerle bağlantı kurarak bağlayın. // Görsel uyarılar için kullanılır
   - Buzzer ve butonları uygun GPIO pinlerine bağlayın. // Sesli uyarı için

3. **Kodları ESP Cihazına Yükleyin:**
   - `Arduino IDE` üzerinden uygun kodları ESP modülüne yükleyin.
   - Wi-Fi bilgilerini ve MQTT Broker adresini kodda düzenleyin. // Ağa bağlanmak ve verileri aktarmak için önemlidir

4. **MQTT Broker’ı Ayarlayın:**
   - HiveMQ, Mosquitto veya Adafruit IO gibi bir MQTT broker kullanın. // Verilerin uzaktan erişilebilmesi için gereklidir
   - ESP modülü, ölçtüğü mesafeyi belirlenen MQTT kanalına gönderecektir.

5. **Mobil/Web Arayüzüne MQTT Aboneliği Yapın:**
   - MQTT client uygulaması (MQTT Explorer, IoT Dashboard vb.) kullanarak verileri gerçek zamanlı takip edin.

## 📜 Proje Lisans Bilgileri
Bu proje MIT Lisansı altında sunulmaktadır. 

## 🔑 Proje Anahtar Kelimeleri
- IoT
- Akıllı Park Sensörü
- ESP32
- ESP8266
- MQTT
- Ultrasonik Sensör
- LED Uyarı Sistemi
- Buzzer
- Arduino

## 📷 Görseller


![Bağlantı Şeması](Figure/diagram.png)

## 📁 Dosya Yapısı
```
AkilliParkSensörü/
│── README.md
│── Figure/
│── OneriRapor/
│   ├── OneriRapor.md
│── AraRapor/
│   ├── AraRapor.md
│   ├── Figure/
│── FinalRapor/
│   ├── FinalRapor.md
│   ├── Figure/
└── Codes/
```
