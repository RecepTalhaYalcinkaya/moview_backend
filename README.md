# 🎬 Film İnceleme ve Favori Listesi API

Bu proje, Flask framework'ü kullanılarak geliştirilmiş bir RESTful API'dir. Kullanıcılar kayıt olabilir, giriş yapabilir, filmleri inceleyebilir, favorilerine film ekleyebilir ve kendi profillerini yönetebilirler.

## 🚀 Özellikler

- ✅ Kullanıcı kayıt ve giriş (JWT tabanlı kimlik doğrulama)
- 👤 Profil görüntüleme ve güncelleme
- 🔒 Parola değiştirme
- 🎥 Film listeleme, arama ve detay görüntüleme
- 📝 İnceleme ekleme, düzenleme ve listeleme
- ⭐ Favorilere film ekleme, listeleme ve silme
- 📚 Kategorileri listeleme
- 🔐 CORS ve bcrypt şifreleme desteği
- 🛑 Global hata yönetimi

📡 API Uç Noktaları
🧑 Kullanıcı İşlemleri
POST /api/users/register → Kullanıcı kaydı

POST /api/users/login → Giriş

GET /api/users/me → Bilgileri al (JWT gerekli)

PUT /api/users/profile → Profil güncelle (JWT gerekli)

PUT /api/users/password → Parola değiştir (JWT gerekli)

🎞️ Filmler
GET /api/movies → Tüm filmleri listele

GET /api/movies/<movie_id> → Film detayları ve incelemeleri

GET /api/movies/search?q=<arama> → Film adına göre arama

📝 İncelemeler
POST /api/reviews → İnceleme ekle (JWT gerekli)

PUT /api/reviews/<review_id> → İnceleme güncelle (JWT gerekli)

GET /api/reviews → Tüm incelemeleri listele

⭐ Favoriler
POST /api/favorites → Favoriye ekle (JWT gerekli)

GET /api/favorites → Favorileri getir (JWT gerekli)

DELETE /api/favorites/<favorite_id> → Favoriden çıkar (JWT gerekli)

📚 Kategoriler
GET /api/categories → Tüm kategorileri getir
