# 🚀 AI Destekli Müşteri ve İş Akışı Yönetim Sistemi

Bu proje, freelancerlar ve dijital ajanslar için e-posta üzerinden gelen müşteri taleplerini **tam otonom** bir şekilde analiz eden, sınıflandıran ve önceliklendiren No-Code/Low-Code tabanlı bir otomasyon sistemidir.

## 📋 Proje Özeti
Yoğun mesaj trafiği arasında kaybolmayı önlemek amacıyla geliştirilen bu sistem; gelen e-postaları insan müdahalesi olmadan okur, bağlamsal analizini yapar ve veritabanına işleyerek yanıt taslaklarını hazırlar. Bu sayede iş gücünden büyük oranda tasarruf sağlar ve yanıt süresini saniyelere indirir.

---

## 🛠 Kullanılan Teknolojiler
Sistem, modern No-Code ve AI araçlarının güçlü bir kombinasyonundan oluşmaktadır:

* **n8n:** Uçtan uca otomasyon akışının (workflow) kurgulanması.
* **Google Gemini 2.5 Flash API:** E-postaların anlamsal analizi ve skorlanması.
* **Google Workspace (Gmail):** Veri kaynağı (Trigger) ve taslak (Draft) yönetimi.
* **Google Sheets:** Dinamik veritabanı yönetimi.
* **Google Sites:** Canlı yönetim paneli (Dashboard) arayüzü.

---

## 🏗 İş Akışı (Workflow) Mimarisi

Proje, birbirine entegre üç ana aşamadan oluşmaktadır. İşte sistemin arka planındaki teknik yapı:

### 1. Tetikleme Mekanizması (Trigger Workflow)
Sistem, Gmail kutusuna düşen yeni mesajları gerçek zamanlı olarak dinler ve analiz sürecini başlatır.
![Trigger Workflow](https://raw.githubusercontent.com/enisecmt/ai-freelance-automation-system/refs/heads/main/Trigger%20Workflow.png)

### 2. Ana İşleme Hattı (Main Workflow)
AI motorunun devreye girdiği, e-postanın kategorize edildiği (Web, Tasarım, Sosyal Medya) ve öncelik skorunun (1-10) belirlendiği merkez yapıdır.
![Ana Workflow](https://raw.githubusercontent.com/enisecmt/ai-freelance-automation-system/refs/heads/main/Ana%20Workflow.png)

### 3. Acil Durum Yönetimi (Emergency Workflow)
Gemini tarafından 8 ve üzeri skor verilen "Kritik" talepler için özel bir akış devreye girer. Bu akış, yöneticinin hızlı aksiyon almasını sağlar.
![Acil Workflow](https://raw.githubusercontent.com/enisecmt/ai-freelance-automation-system/refs/heads/main/Acil%20Workflow.png)

---

## ✨ Temel Özellikler
* **Bağlamsal AI Analizi:** Karmaşık metinleri analiz ederek 2 cümlelik özetler çıkarır.
* **Akıllı Önceliklendirme:** Acil işleri anında tespit ederek "Acil İşler Akışını" tetikler.
* **Otomatik Yanıt Taslağı:** Talebe özel, profesyonel bir dil ile hazırlanmış yanıtı doğrudan Gmail "Taslaklar" klasörüne kaydeder.
* **Canlı Dashboard:** Tüm süreci Google Sites üzerinden hazırlanan şık bir panelden izleme imkanı sunar.

---

## 📖 Kullanım Senaryosu
1.  **Talep:** Bir müşteri "Sitemiz çöktü, acil destek!" konulu bir mail atar.
2.  **İşleme:** n8n akışı 15 saniye içinde maili Gemini'ye gönderir. Gemini maili 10/10 aciliyetle puanlar.
3.  **Kayıt:** Veriler Google Sheets'e işlenir ve profesyonel bir yanıt taslağı Gmail'de oluşturulur.
4.  **Onay:** Yönetici, Dashboard üzerinden bildirimi görür, taslağı kontrol eder ve tek tıkla gönderir.

---

## 👤 Geliştirici
**Enise Cömet**
