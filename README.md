# BMÜ329 Veri Tabanı Sistemleri Dersi Dönem Projesi Gereksinimleri ve E-R Diyagramı

## Proje Başlığı: Endüstriyel Otomasyon ve Haberleşme Ürünleri Yönetim Sistemi

**Proje Ekibindeki Kişiler:**
- **220260020** - Muhammed Salih Üstün
- **220260054** - Emre Gülek
- **220260092** - Muhammed Gökhan Şentürk

---

## Endüstriyel Otomasyon ve Haberleşme Ürünleri Yönetim Sistemi

## 1. Cihaz ve Kategori Yönetimi

### Categories (Kategoriler)
Cihazların ait olduğu ana kategorileri tanımlamak için kullanılır. Her kategorinin:
- **CategoryID**: Benzersiz kimlik numarası
- **Adı**: Kategorinin adı
- **Tanımı**: İsteğe bağlı açıklama bilgisi bulunur.

### DeviceSeries (Cihaz Serileri)
Cihazlar, bir kategoriye ait belirli serilere ayrılır. Bu tabloda:
- **SeriesID**: Serinin benzersiz kimliği
- **Adı**: Seri adı
- **Açıklama**: Seriye dair açıklama bilgileri bulunur.
- **CategoryID**: Kategorilerle bağlantılıdır.

### Devices (Cihazlar)
Sistemde yer alan tüm cihazları tanımlar. Her cihaz:
- **SeriesID**: İlgili seriyle ilişkilidir.
- **Adı**: Cihazın adı
- **Özellikleri**: Teknik ve donanımsal özellikler
- **Üretim Tarihi**: Cihazın üretim tarihi
- **Açıklama**: Detaylı açıklama bilgilerini içerir.

---

## 2. Kullanıcı ve Destek Yönetimi

### Users (Kullanıcılar)
Sistemdeki tüm kullanıcıları temsil eder. Kullanıcı bilgileri şunlardır:
- **Kullanıcı Adı**
- **E-posta**
- **Şifre**
- **Son Giriş Tarihi**

### CustomerSupport (Müşteri Destek)
Kullanıcıların sistemde oluşturduğu destek kayıtlarını tutar. Her kayıt:
- **UserID**: Destek talebini oluşturan kullanıcı
- **Destek Tarihi**: Talebin tarihi
- **Talep Açıklaması**: Destek isteğine dair detayları içerir.

### CustomerSupportTechnician (Destek Teknisyenleri)
Destek taleplerini yöneten teknisyenlerin bilgilerini içerir. Bu bilgiler:
- **SupportID**: İlgili destek kaydı
- **Teknisyen Adı**
- **Pozisyonu**
- **Tecrübesi** gibi ayrıntılardır.

---

## 3. Cihaz Teknik ve Donanım Yetenekleri

### DeviceFeatures (Cihaz Özellikleri)
Cihazların yazılım ve donanım yeteneklerini belirtir. Özellikler arasında:
- **IEC 61131-3 Standardına Uygunluk**
- **IoT Desteği**
- **USB Programlama** gibi bilgiler bulunur.

### MotionControlFunctions (Hareket Kontrol Fonksiyonları)
Cihazların hareket kontrol yeteneklerini içerir:
- **Hızlı Sayıcı Girişi**
- **PWM Çıkışı** gibi bilgiler burada tanımlanır.

### Programming (Programlama)
Cihazların desteklediği:
- **Programlama Dilleri**
- **Editör Türleri**
- **USB Port Bilgileri** bu tabloda bulunur.

### LEDSignals (LED Sinyalleri)
Cihaz üzerindeki LED sinyallerini belirtir:
- **Güç LED’i**
- **Haberleşme LED’leri** gibi durumlar tanımlanır.

### ElectricalWiring (Elektrik Tesisatı)
Cihazların IO ve güç bağlantılarıyla ilgili bilgileri saklar.

---

## 4. Haberleşme ve Protokol Yönetimi

### CommunicationProtocols (Haberleşme Protokolleri)
Cihazların desteklediği ana protokolleri içerir:
- **Modbus**
- **TCP/IP**
- **IoT Protokolleri**

### CommunicationPorts (Haberleşme Portları)
Cihazların:
- **Ethernet Portları**
- **GSM Haberleşme Portları** gibi bilgilerini içerir.

### GSMFunctions (GSM Fonksiyonları)
GSM ile ilgili özellikler:
- **SMS Gönderim/Alımı**
- **DTMF Aramaları** gibi fonksiyonları içerir.

---

## 5. Garanti ve Sertifikasyon

### Warranty_Certification (Garanti ve Sertifikasyon)
Cihazların garanti ve sertifikasyon bilgilerini içerir:
- **Garanti Süresi**
- **IEC Standartları** gibi detaylar yer alır.

---

## 6. Sipariş Yönetimi

### Orders (Siparişler)
Kullanıcıların verdiği siparişleri saklar:
- **Sipariş Durumu**
- **Toplam Tutar**
- **Oluşturulma Tarihi** bilgilerini içerir.

### OrderDetails (Sipariş Detayları)
Siparişlerde yer alan cihazların bilgilerini içerir:
- **Cihaz Adedi**
- **Sipariş ile Cihazların Bağlantısı**

---

## 7. Çözüm ve Otomasyon Yönetimi

### Solutions (Çözümler)
Cihazlarla ilgili geliştirilen çözümleri içerir:
- **Cihaz İlişkisi**
- **Oluşturulma Tarihi** bilgilerini saklar.

---

## E-R DİYAGRAMI

![E-R Diyagramı](https://github.com/user-attachments/assets/743ed616-130e-4b7c-9b1d-2a8b69ac90f2)




