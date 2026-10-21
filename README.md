# argon-3
# 🚀 Argon 3 — Gelişmiş Mobil AI Asistanı (v0.4)

> **"Geleceğin mobil asistan deneyimini, sistemin derinliklerinden kullanıcı arayüzüne kadar yeniden tanımlıyoruz."**

---

## 👨‍💻 Geliştirici & Proje Hakkında

**Argon 3**, **Çağatay Baltacı** tarafından temelleri atılmış, **3 yılı aşkın süredir** aralıksız geliştirilen, evrimleşen ve olgunlaşan bağımsız bir yapay zeka ve sistem otomasyonu projesidir. 

İlk günlerinde basit bir konsept ve prototip olarak başlayan bu yolculuk; geçen 3 yıllık süreçte sürekli yeni mimariler, arayüz deneyimleri ve mobil optimizasyonlarla zenginleştirilerek günümüzdeki **Argon 3 v0.4** sürümüne ulaşmıştır. 

Projenin ana felsefesi; ağır masaüstü bağımlılıklarını ve hantal yapıları bir kenara bırakıp, mobil cihazlarda minimum kaynak tüketimiyle çalışan, yüksek performanslı ve özgürleştiren bir asistan altyapısı sunmaktır.

---

## 📌 Proje Künyesi

| Bilgi | Detay |
| :--- | :--- |
| **Proje Adı** | Argon 3 |
| **Geliştirici** | Çağatay Baltacı |
| **Geliştirme Süresi** | 3 Yıl+ (Sürekli Aktif Proje) |
| **Mevcut Sürüm** | `v0.4` |
| **Temel Teknolojiler** | Python 3.10, Kivy Framework, Buildozer |
| **Hedef Platform** | Android (Öncelikli), Cross-Platform |
| **Dağıtım Hattı** | GitHub Actions (CI/CD Automated Cloud Build) |

---

## 🛠️ Mimari ve Teknolojik Altyapı

Argon 3, 3 yıllık geliştirme tecrübesinin ışığında mobil öncelikli bir mimari üzerine kurulmuştur:

* 📱 **Kivy Framework (UI/UX):** Dokunmatik ekran dinamiklerine özel olarak tasarlanmış, akıcı sohbet geçmişi (scrolling) ve esnek girdi panelleri sağlayan Python tabanlı grafik arayüzü.
* ⚙️ **Konfigürasyon Esnekliği (`buildozer.spec`):** Özelleştirilmiş paket ismi (`org.argon.argon3`), dinamik izin yönetimi ve optimize edilmiş ekran yönelim ayarları.
* ☁️ **Bulut Tabanlı CI/CD (GitHub Actions):** Yerel ortamlardaki Linux/WSL kurulum karmaşalarını ortadan kaldıran, bulut sunucularda otomatik `.apk` derleme altyapısı.

---

## ⚡ Bulut Derleme ve Otomasyon Mimarisi

Argon 3 projesi, kod değişiklikleri GitHub deposuna gönderildiği an çalışan tam otomatik bir bulut derleme boru hattına (pipeline) sahiptir:

```mermaid
graph TD
    A[VS Code / Geliştirme Ortamı] -->|Git Push| B[GitHub Deposu]
    B -->|Workflow Tetiklenir| C[Ubuntu Bulut Sunucusu]
    C -->|Buildozer Derleme| D[Android APK Paketleme]
    D -->|Artifact Üretimi| E[İndirilebilir Argon 3 APK]
