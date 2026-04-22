# KULLANIM DOKÜMANTASYONU

**Proje Adı:** AI Destekli Müşteri ve İş Akışı Yönetim Sistemi
**Geliştirici:** Enise Cömet

## 1. Proje Özeti
Bu proje, bir freelancerın veya dijital ajansın e-posta üzerinden aldığı müşteri taleplerini insan eli değmeden analiz eden, sınıflandıran, önceliklendiren ve veritabanına kaydeden No-Code/Low-Code tabanlı bir otomasyon sistemidir. Yapay zeka entegrasyonu sayesinde yoğun mesaj trafiği saniyeler içinde filtrelenir ve iş gücünden büyük oranda tasarruf sağlanır.

## 2. Kullanılan Teknolojiler ve Araçlar
*   **n8n (No-Code Platform):** Uçtan uca otomasyon akışının (workflow) kurgulanması ve yönetimi.
*   **Google Gemini 2.5 Flash API:** E-postaların anlamsal analizi, skorlanması ve yanıt taslağı üretilmesi.
*   **Google Workspace (Gmail):** Veri kaynağı (Trigger) ve çıktı (Draft) entegrasyonu.
*   **Google Sheets:** Dinamik veritabanı yönetimi.
*   **Google Sites:** Yönetim paneli (Dashboard) arayüzünün oluşturulması.

## 3. Sistemin Temel Özellikleri ve Yetenekleri
*   **Sıfır Temaslı Kayıt:** E-posta kutusuna düşen her yeni talep otomatik olarak yakalanır.
*   **Bağlamsal AI Analizi:** Karmaşık e-posta metinleri okunarak; *Kategori* (Web, Tasarım, Sosyal Medya), *Öncelik Skoru* (1-10 arası) ve 2 cümlelik *Özet* haline getirilir.
*   **Akıllı Yönlendirme (Routing):** Yapay zekanın verdiği Öncelik Skoru 8 ve üzeri olan talepler için sistem ikili bir yol ayrımına (IF yapısı) girerek "Acil İşler Akışını" tetikler.
*   **Otomatik Yanıt Taslağı:** Yapay zeka, talebin içeriğine özel ve profesyonel bir "İlk Yanıt Taslağı" hazırlar ve bunu direkt olarak kullanıcının Gmail Taslaklar klasörüne kaydeder.
*   **Canlı Dashboard Arayüzü:** Tüm bu süreç, Google Sites üzerinde hazırlanan şık bir panelden tek ekranda canlı olarak izlenebilir.

## 4. Kullanım Adımları (Örnek Senaryo)
1. **Tetiklenme:** Müşteri, projeye özel tanımlanmış olan e-posta adresine bir talep maili atar *(Örn: "Acil e-ticaret sitemiz çöktü")*.
2. **Arka Plan İşlemi (15 Saniye):** n8n akışı devreye girer. E-postayı alır, Gemini'ye gönderir, skoru hesaplar (Örn: 10/10), Google Sheets'e yazar ve Gmail'de taslağı oluşturur.
3. **İzleme ve Yönetim:** Sistem yöneticisi, Google Sites üzerinden "AI Müşteri Yönetim Paneli"ne girer. Burada yeni talebin konusunu, yapay zekanın çıkardığı özeti ve "Çok Acil" uyarı skorunu görür.
4. **Aksiyon Alma:** Yönetici, paneldeki taslağın hazır olduğunu gördükten sonra tek tıkla Gmail "Taslaklar" kutusuna girer. Yapay zekanın yazdığı profesyonel cevabı kontrol eder ve "Gönder" butonuna basarak işi saniyeler içinde tamamlar.

## 5. Başarı ve Sonuç
Bu sistem, karmaşık ve zaman alan "Müşteri iletişim ve tasnif" sürecini tam otonom bir yapıya kavuşturmuştur. "No-Code" araçların "AI" ile doğru entegre edildiğinde gerçek bir iş problemini ne kadar hızlı ve verimli çözebileceğinin çalışan bir kanıtıdır.
