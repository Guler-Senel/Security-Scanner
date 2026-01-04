# GuvenlikTarayici (Security Scanner)

GuvenlikTarayici, C# Windows Forms kullanılarak geliştirilmiş, **eğitim amaçlı bir dosya güvenlik tarayıcısıdır**.  
Uygulama, seçilen bir klasörü (alt klasörler dahil) tarayarak potansiyel olarak şüpheli dosyaları tespit etmeyi ve bu dosyaları karantinaya almayı amaçlar.

## Proje Amacı
Bu projenin amacı, temel dosya analiz yaklaşımlarını (heuristic analiz ve hash tabanlı kontrol) uygulamalı olarak göstermek ve masaüstü uygulamalarında güvenlik odaklı bir mimarinin nasıl kurulabileceğini örneklemektir.

> **Not:** Bu uygulama gerçek bir antivirüs yazılımı değildir. Eğitim ve demonstrasyon amaçlıdır.

## Temel Özellikler
- Klasör ve alt klasörler dahil dosya tarama
- Uzantı tabanlı şüpheli dosya tespiti
- Dosya adı anahtar kelime analizi (heuristic yaklaşım)
- Küçük boyutlu çalıştırılabilir dosyalar için ek kontrol
- SHA256 hash hesaplama
- Demo amaçlı blacklist / whitelist desteği
- Tarama sürecini gösteren ProgressBar
- Şüpheli dosyalar için karantina sistemi
- Karantina işlemleri için loglama (log.txt)

## Kullanım Adımları
1. Uygulamayı çalıştırın.
2. **Klasör Seç / Select Folder** butonu ile taranacak klasörü belirleyin.
3. **Tara / Scan** butonuna basarak taramayı başlatın.
4. Şüpheli dosyalar tespit edilirse **Karantinaya Al / Quarantine** butonu aktif hale gelir.
5. Karantinaya alınan dosyalar, seçilen klasör içinde oluşturulan `Quarantine` klasörüne taşınır.

## Teknik Detaylar
- Geliştirme Dili: **C#**
- Uygulama Türü: **Windows Forms**
- Framework: **.NET 6 / .NET 8**
- Hash Algoritması: **SHA256**
- Platform: **Windows**

## Sınırlamalar
- Gerçek zamanlı koruma sağlamaz.
- Güncel zararlı imza veritabanı içermez.
- Gelişmiş davranışsal analiz yapılmamaktadır.

## Sonuç
GuvenlikTarayici projesi, dosya güvenliği ve temel antivirüs mantığını kavramaya yönelik, akademik ve öğretici bir masaüstü uygulama örneğidir.

