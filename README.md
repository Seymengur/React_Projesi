# dotcom eğitim - React & TSX Mimari Eğitimi

Modern web teknolojilerini sıfırdan ileri seviyeye öğretmeyi hedefleyen, React ve TypeScript ile geliştirilmiş interaktif bir eğitim platformu arayüzüdür. Bu proje, "Bileşen Tabanlı Web Geliştirme" ödev gereksinimlerini karşılamak amacıyla tasarlanmıştır.

## Proje Amacı

Kullanıcılara React, TypeScript, Hooks, Form Yönetimi, Performans Optimizasyonları ve İleri Düzey Mimari desenlerini interaktif ve okunabilir bir arayüzle sunmak.

## Öne Çıkan Özellikler (Ödev Gereksinimleri)

* **Modern React & TSX:** Tamamen fonksiyonel bileşenler (Functional Components) ve React Hooks (`useState`, vb.) kullanılarak inşa edilmiştir.
* **Tip Güvenliği:** Veri modelleri ve component propları için kapsamlı TypeScript `interface` ve `type` tanımlamaları yapılmıştır (`index.ts`).
* **Modüler Bileşen Mimarisi:** Uygulama Navbar, Sidebar, Content, Footer gibi mantıksal ve yeniden kullanılabilir parçalara ayrılmıştır.
* **Etkileşim:** Menüler arası dinamik geçişler, aktif konu takibi ve "Kodu Kopyala" gibi etkileşimli özellikler mevcuttur.
* **Modern UI/UX & Responsive Tasarım:** CSS Değişkenleri (CSS variables) ile kurumsal bir renk paleti oluşturulmuş, `@media` sorguları ile mobil, tablet ve masaüstü cihazlara tam uyum sağlanmıştır. Mac tarzı kod blokları ile okuma deneyimi iyileştirilmiştir.
* **Zengin İçerik:** 600 satırdan fazla, özenle hazırlanmış ve kategorize edilmiş React müfredatı içermektedir.

## 🛠️ Kullanılan Teknolojiler

* **Kütüphane:** React 18
* **Dil:** TypeScript
* **Stil:** Saf CSS (Custom CSS Variables & Flexbox/Grid Layouts)
* **İkonlar:** Inline SVG

## Proje Yapısı

/ (Proje Kök Dizini)
├── public/                # Statik dosyalar (Favicon vb.)
├── src/                   # Uygulama kaynak kodları
│   ├── components/
│   │   ├── Footer.tsx         # Kapsamlı ve şık alt bilgi
│   │   ├── HomePage.tsx       # Eğitim setlerinin listelendiği karşılama ekranı
│   │   ├── LeftSidebar.tsx    # Konu başlıklarının bulunduğu sol menü
│   │   ├── MainContent.tsx    # Konu anlatımı ve kod örneklerinin sunulduğu ana alan
│   │   ├── RightSidebar.tsx   # Reklam/Ekstra araçların bulunduğu sağ menü
│   │   ├── TopicCard.tsx      # Yeniden kullanılabilir konu kartı
│   │   └── TopNavbar.tsx      # Üst navigasyon barı
│   ├── data/
│   │   └── reactCurriculum.ts # Kategorize edilmiş dev müfredat verisi
│   ├── types/
│   │   └── index.ts           # Global TypeScript interface tanımları
│   ├── App.tsx                # Ana layout ve durum yönetimi
│   ├── index.css              # Global stiller ve responsive kurallar
│   └── main.tsx               # React giriş noktası
├── .gitignore             # Git versiyon kontrolü dışında bırakılacak dosyalar
├── eslint.config.js       # ESLint kod kalite ve standartları yapılandırması
├── index.html             # Vite için ana HTML şablonu
├── package.json           # Proje bağımlılıkları ve scriptleri
├── package-lock.json      # Bağımlılık ağacının kilit dosyası
├── README.md              # Proje dökümantasyonu
├── tsconfig.app.json      # Uygulama içi TypeScript yapılandırması
├── tsconfig.json          # Ana TypeScript yapılandırması
├── tsconfig.node.json     # Vite/Node ortamı için TS yapılandırması
└── vite.config.ts         # Vite derleyici ve sunucu yapılandırması

*(Not: `node_modules` klasörü bağımlılıkları içerir ve proje teslim/boyut optimizasyonu için versiyon kontrolüne dahil edilmemiştir.)*


## Kurulum ve Çalıştırma

Projeyi yerel ortamınızda çalıştırmak için aşağıdaki adımları izleyebilirsiniz:

1. Proje dosyalarını bilgisayarınıza indirin (veya zip'ten çıkarın).
2. Terminal (veya Komut İstemcisi) üzerinden proje dizinine gidin.
3. Gerekli bağımlılıkları yüklemek için aşağıdaki komutu çalıştırın:
   bash
   npm install

4. Geliştirme sunucusunu başlatmak için aşağıdaki komutu çalıştırın:
   bash
   npm run dev
5. Tarayıcınızda, terminalde belirtilen adrese (`http://localhost:5173`) giderek projeyi görüntüleyebilirsiniz.