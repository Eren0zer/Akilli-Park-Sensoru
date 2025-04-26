# 📌 Akıllı Park Sensörü - Ara Raporu

## Grup Bilgileri
**Grup 1**  
İlhan Emre Adak  
Sıdıka Firat  
Eren Özer  
Şevval Yavuz
<br><br>
## 1. Proje Konusu

Günümüz araç güvenlik sistemleri, sürücülerin park ve manevra işlemlerinde desteklenmesi amacıyla çeşitli sensör ve kamera teknolojilerinden yararlanmaktadır. Bu kapsamda geliştirilen proje, ultrasonik sensör aracılığıyla aracın çevresindeki mesafelerin tespit edilmesini ve sürücüye hem görsel (LED) hem de işitsel (buzzer) uyarılar sunulmasını amaçlamaktadır. Bunun yanı sıra, ilerleyen aşamalarda ESP32-CAM modülü kullanılarak aracın bulunduğu ortamın görüntüsünün alınması ve bu görüntünün kablosuz iletişim yoluyla aktarılması hedeflenmektedir. Böylelikle kullanıcıya yalnızca mesafe değil, aynı zamanda çevresel durum hakkında da anlık bilgi sunularak, sistemin işlevselliği artırılacaktır.
<br><br>

## 2. Özet

Projenin bu aşamasında temel donanımsal altyapı oluşturulmuş ve sistemin ilk işlevsellik testleri başarıyla tamamlanmıştır. Arduino Uno geliştirme kartı kullanılarak HC-SR04 ultrasonik sensörü ile cismin uzaklığı ölçülmüş; ölçüm sonuçlarına göre farklı renklerde LED’lerin (yeşil, sarı, kırmızı) yanması ve belirli kritik eşik değerlerinde buzzer’ın devreye girerek sürücüye sesli uyarı vermesi sağlanmıştır. Bu yapı, sürücünün çevresel mesafeleri algılayarak daha güvenli park ve manevra yapmasını desteklemek amacıyla tasarlanmıştır.
<br><br>
## 3. Kullanılan Yöntemler

- **Ultrasonik Mesafe Ölçümü:** HC-SR04 sensörü kullanılarak cismin uzaklığı ölçülmüştür.
- **Görsel Uyarı Sistemi:** Farklı mesafelerde farklı renklerde LED’ler yanacak şekilde tasarlanmıştır.
- **İşitsel Uyarı Sistemi:** Kritik mesafe aşıldığında buzzer devreye girerek sesli uyarı verilmiştir.
- **Arduino Programlama:** Arduino IDE kullanılarak, tüm sensör ve çıkış birimleri kod ile kontrol edilmiştir.
- **Donanım Montajı:** Breadboard ve jumper kablolar ile prototip devre kurulmuştur.
- **ESP32-CAM Planlaması:** Gelecek aşamalarda görüntü aktarımı için ESP32-CAM modülü sisteme entegre edilecektir.
<br><br>
## 4. Yapılan Çalışmalar ve Görselleri

### 4.1 Kullanılan Parçalar

| Parça | Görsel |
|:-----|:------:|
| Arduino Uno | ![Arduino Uno](./Figure/arduino_uno.jpg) |
| HC-SR04 Ultrasonik Sensör | ![HC-SR04](./Figure/hc_sr04.jpg) |
| LED'ler ve Buzzer | ![LED ve Buzzer](./Figure/led_buzzer.jpg) |
| Breadboard ve Jumper Kablolar | ![Breadboard](./Figure/breadboard.jpg) |

### 4.2 Devre Şeması

| Devre Şeması |
|:------------:|
| ![Devre Şeması](./Figure/devre_semasi.jpg) |

### 4.3 Proje Fotoğrafları

| Sistem Kurulumu | Test Anı | Yakın Çekim |
|:---------------:|:--------:|:-----------:|
| ![Devre Kurulumu](./Figure/devre_kurulumu.jpg) | ![Çalışma Testi](./Figure/mesafe_test.jpg) | ![Yakın Çekim](./Figure/yakin_cekim.jpg) |

### 4.4 Çalışır Sistem Videosu

📹 [Sistem Çalışma Videosu (İzlemek için tıklayın)](https://www.youtube.com/shorts/-A3FBNeWkMM?feature=share)
<br>
(Not: LED'lerin videoda daha net görünebilmesi için sadece video çekimi sırasında LED'lere bağlı dirençler çıkarılmıştır.)
<br><br>
## 5. Elde Edilen Sonuçlar

| Test Edilen Özellik | Gözlemler ve Sonuçlar |
|:-------------------|:----------------------|
| Ultrasonik Sensör ile Mesafe Ölçümü | Ölçümler doğru ve tutarlı, sapma ±2 cm civarındadır. |
| LED ile Görsel Uyarı Sistemi | LED'ler doğru mesafe eşiklerinde aktive olmuştur. |
| Buzzer ile İşitsel Uyarı Sistemi | Buzzer doğru kritik mesafe aralığında çalışmıştır. |
| Donanım Stabilitesi | Ufak temas problemleri dışında sistem stabil çalışmıştır. |
| Arduino Yazılımı Performansı | Düşük gecikme ile giriş-çıkış tepkileri alınmıştır. | <br><br>br><br>
## 6. Karşılaşılan Sorunlar ve Çözümler

| Sorun | Çözüm |
|:-----|:------|
| Breadboard Alanının Yetersizliği | Kısa jumper kablolarla bağlantılar düzenlendi, kritik devreler doğrudan Arduino’ya bağlandı. |
| Yanlış Sensör Bağlantıları | Sensör bağlantıları veri sayfası yardımıyla yeniden yapıldı. |
| LED'lerin Yanlış Koşullarda Çalışması | Yazılım koşulları ve mesafe aralıkları yeniden düzenlendi. |
| Buzzer'ın Zamansız Çalışması | Kritik mesafe eşikleri optimize edildi. |
| Temas Problemleri | Bağlantılar elle sabitlendi ve sıkılaştırıldı. | <br><br>br><br>



## 7. Projenin Devamında Yapılacaklar

- **ESP32-CAM Kurulumu ve Programlanması:** Arduino IDE üzerinde yapılandırılacak ve temel bağlantı testleri yapılacaktır.
- **Wi-Fi Bağlantısının Sağlanması:** ESP32-CAM’in Wi-Fi ağına bağlanması sağlanacaktır.
- **Görüntü Alımı:** Ortam görüntüsü yakalanarak kayıt altına alınacaktır.
- **Görüntü Aktarımı:** Alınan görüntü belirlenen istemciye (web veya mobil cihaz) aktarılacaktır.
- **Sistem Entegrasyonu:** ESP32-CAM görüntü sistemi ve mevcut Arduino Uno sistemi entegre şekilde çalışacaktır.
<br><br>


## 8. Ticari Değerlendirme

Bu proje, düşük maliyetli ve basit montaj imkanı sunan yapısı sayesinde ticari olarak çeşitli alanlarda değerlendirilebilir. Özellikle eski model araçlara kolayca entegre edilerek sürücülere ek güvenlik sağlanabilir. Ayrıca küçük otopark işletmeleri için düşük bütçeli park destek sistemleri geliştirmek amacıyla kullanılabilir. Projenin modüler yapısı sayesinde ihtiyaçlara göre genişletilmesi ve özelleştirilmesi mümkündür, bu da onu pazarlanabilir bir ürün haline getirmektedir.

---


# Dosya Yapısı

```
AraRapor/
│── AraRapor.md
│── Figure/
│   ├── arduino_uno.jpg
│   ├── hc_sr04.jpg
│   ├── led_buzzer.jpg
│   ├── breadboard.jpg
│   ├── devre_kurulumu.jpg
│   ├── mesafe_test.jpg
│   ├── yakin_cekim.jpg
│   ├── devre_semasi.jpg
│   ├── sistem_test_videosu.mp4
```

