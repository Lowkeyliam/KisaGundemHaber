# Kısa Gündem 📰

Günlük haber başlıklarını kısa özetlerle sunan, reels tarzında kaydırılabilir modern web uygulaması.

## ✨ Özellikler

### 📱 **Kullanıcı Deneyimi**
- **Reels Tarzı Deneyim**: Haberleri yukarı/aşağı kaydırarak gezinebilirsiniz
- **Akıllı Arama**: Başlık, içerik ve kaynak bazlı gerçek zamanlı arama
- **PWA Desteği**: Mobil cihazlara uygulama olarak yüklenebilir
- **Offline Çalışma**: Service Worker ile internet bağlantısı olmadan kullanım

### 🗂️ **İçerik Yönetimi**
- **9 Kategori**: Spor, Politika, Ekonomi, Teknoloji, Sağlık, Eğitim, Güvenlik, Hava & Doğa, Kültür & Sanat
- **RSS Beslemesi**: Türkiye'nin önde gelen haber kaynaklarından otomatik güncelleme
- **Sınırsız Haber**: RSS'den gelen tüm haberler gösterilir
- **Gerçek Zamanlı**: 15 dakikada bir otomatik güncelleme

### ⌨️ **Gelişmiş Kontroller**
- **Klavye Kısayolları**: J/K (Vim tarzı), ok tuşları, boşluk tuşu ile navigasyon
- **Hızlı Arama**: / tuşu ile arama kutusuna odaklanma
- **Tema Değiştirme**: D tuşu ile hızlı dark mode geçişi
- **Otomatik Kaydırma**: 8 saniyede bir otomatik haber geçişi (isteğe bağlı)

## 🚀 Kurulum

1. **Depoyu klonlayın**
```bash
git clone [https://github.com/erent8/KisaGundemHaber/tree/main]
cd KısaGundemHaber
```

2. **Bağımlılıkları yükleyin**
```bash
npm install
```

3. **Uygulamayı başlatın**
```bash
npm start
```

4. **Tarayıcıda açın**
```
http://localhost:3000
```

## 🎮 Kullanım

### Navigasyon Yöntemleri:
- **Klavye**: ↑↓ ok tuşları, J/K tuşları (Vim tarzı), boşluk tuşu
- **Mouse**: Fare tekerleği
- **Dokunmatik**: Yukarı/aşağı kaydırma (swipe)
- **Butonlar**: Sağ taraftaki navigasyon okları
- **Kategori Filtreleme**: Header altındaki renkli kategori butonları

### Gelişmiş Kısayollar:
- **J** / **↓** / **Space** - Sonraki haber
- **K** / **↑** - Önceki haber
- **/** - Arama kutusuna odaklan
- **Esc** - Aramayı temizle ve odağı kaldır
- **R** - Haberleri yenile

### Arama Özellikleri:
- **Gerçek zamanlı filtreleme** - Yazdıkça sonuçlar güncellenir
- **Çoklu alan arama** - Başlık, içerik ve kaynak arama
- **Vurgulama** - Bulunan kelimeler sarı ile işaretlenir
- **Hızlı temizleme** - X butonu ile aramayı temizleme

## 📱 Haber Kaynakları

Uygulama aşağıdaki RSS kaynaklarından haberler çeker:
- BBC Türkçe
- NTV
- CNN Türk
- Hürriyet
- Sabah

## 📸 Ekran Görüntüleri 
<img width="1918" height="902" alt="gundem1" src="https://github.com/user-attachments/assets/205acbab-6d55-4a1b-adea-5c35cef2ddcd" />
<img width="1918" height="910" alt="2" src="https://github.com/user-attachments/assets/0b23eccc-30dd-448f-9e83-d521733da0d3" />
<img width="1918" height="902" alt="gundem3" src="https://github.com/user-attachments/assets/5d9aac33-bf42-4f02-8111-1c5b7d416914" />
<img width="1918" height="905" alt="tttt" src="https://github.com/user-attachments/assets/8609411b-31e4-4713-8c91-b02a695b0f5e" />


## ⚙️ Teknik Detaylar

### Backend:
- **Node.js** + Express
- **RSS Parser** - Haber beslemelerini işler
- **Node Cron** - 15 dakikada bir otomatik güncelleme

### Frontend:
- **Vanilla JavaScript** - Hafif ve hızlı
- **CSS3** - Modern animasyonlar ve geçişler
- **Service Worker** - PWA desteği

### Özellikler:
- **Otomatik Güncelleme**: 15 dakikada bir RSS kaynaklarından yeni haberler çeker
- **Bellek İçi Depolama**: Hızlı erişim için haberler bellekte tutulur
- **Hata Yönetimi**: RSS kaynaklarında hata olması durumunda diğer kaynaklardan devam eder

## 🔧 Geliştirme

```bash
# Geliştirme modunda çalıştır (nodemon ile)
npm run dev
```

## 📄 Lisans

MIT License

## 🛣️ Roadmap

### Yakın Gelecek (v1.1-1.3)
- 🎨 **UI/UX İyileştirmeleri**: Animasyonlar, kullanıcı tercihleri, erişilebilirlik
- 📊 **Analytics**: Okuma istatistikleri, trending haberler, kullanıcı dashboard'u  
- 🔧 **Performans**: Lazy loading, veritabanı entegrasyonu, hata yönetimi

### Orta Vadeli (v2.0+)
- 🌐 **Sosyal Özellikler**: Paylaşım sistemi, topluluk özellikleri
- 🤖 **AI Entegrasyonu**: Haber özetleme, sentiment analysis, kişiselleştirme
- 📱 **Platform Genişletmesi**: Desktop app, Chrome extension, API geliştirme

Detaylı roadmap için [ROADMAP.md](ROADMAP.md) dosyasını inceleyin.

## 🤝 Katkıda Bulunma

Bu açık kaynak projeye katkılarınızı bekliyoruz! 

### Hızlı Başlangıç
1. **Fork** edin ve **clone** yapın
2. **Feature branch** oluşturun (`git checkout -b feature/yeniOzellik`)
3. **Değişikliklerinizi** yapın ve test edin
4. **Commit** edin (`git commit -am 'feat: yeni özellik eklendi'`)
5. **Push** edin (`git push origin feature/yeniOzellik`)
6. **Pull Request** oluşturun

### Katkı Türleri
- 🐛 **Bug Report**: Hata bildirimi
- 💡 **Feature Request**: Yeni özellik önerisi
- 💻 **Code Contribution**: Kod katkısı
- 📚 **Documentation**: Dokümantasyon iyileştirme
- 🎨 **Design**: UI/UX tasarım önerileri
- 🌍 **Translation**: Çeviri katkısı

Detaylı katkı rehberi için [CONTRIBUTING.md](CONTRIBUTING.md) dosyasını okuyun.

## 📋 Geliştirme Kuralları

Proje [.cursorrules](.cursorrules) dosyasında tanımlanan kod standartlarını takip eder:
- ES6+ JavaScript syntax
- Mobile-first responsive design  
- Accessibility standartları
- PWA best practices
- Dark mode desteği

## 📄 Lisans

MIT License - Detaylar için [LICENSE](LICENSE) dosyasını inceleyin.

## 🙏 Teşekkürler

- **RSS Kaynaklarına**: BBC Türkçe, NTV, CNN Türk, Hürriyet, Sabah
- **Açık Kaynak Topluluğuna**: Kullanılan kütüphaneler için
- **Katkıda Bulunanlara**: Her türlü katkı için

## 📧 İletişim

- **Issues**: GitHub Issues üzerinden
- **Discussions**: Genel tartışmalar için GitHub Discussions
- **Email**: Acil durumlar için [erenterzi@protonmail.com]

---

**⭐ Beğendiyseniz projeye yıldız vermeyi unutmayın!**
