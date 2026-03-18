# Proje Bilgileri 
1) Proje özeti
 - **İsim:** Personal Valut 
 - **Amaç:** Kullanıcıların almış olduğu notları uçtan uca şifreleyip her kullanıcı için hesap oluşturma. Ayrıca kullanıcının isteği doğrultusunda kendisinin uygulamayı özelleştirebilmesi. 
 - **Hedef:** Gizllilik ve not almaya önem veren kişiler 

2) Teknik Yığın (Tech Stack): 
 - **Framework:** Flutter 
 - **State Management:** Riverpod
 - **Veritabanları:** Yerelde 'Isar' , Bulut senkronizasyonu için 'Firebase'
 - **Servisler:** `get_it` (Dependency Injection için).

3) Dosya Yapısı: 
- `lib/models/`: Veri modelleri ve JSON serileştirme.
- `lib/screens/`: UI sayfaları.
- `lib/widgets/`: Tekrar kullanılabilir küçük widget'lar.
- `lib/services/`: API, DB ve Auth servisleri.
- `lib/providers/`: State yönetimi logic'leri.

4) Kod Yazma standartları: 
- **İsimlendirme:** Sınıflar `PascalCase`, değişkenler ve metotlar `camelCase`, dosya isimleri `snake_case` olmalı.
- **Widget Yapısı:** Mümkün olduğunca `const` constructor kullanılmalı.
- **Hata Yönetimi:** Tüm servis çağrıları `try-catch` blokları içinde ele alınmalı.
- **Linting:** `flutter_lints` kurallarına sıkı sıkıya uyulmalı.
- **Asenkron:** `Future` ve `Stream` işlemleri temiz bir şekilde yönetilmeli.

5) Kritik Modüller
- `auth_service.dart`: Kullanıcı giriş/çıkış işlemlerini yönetir.
- `sync_engine.dart`: Yerel veri ile bulut verisini eşitleyen ana motor.

6) Notlar: 
- Bu dosyada bahsedilipte yazılmamış olan dosyalar varsa kendin oluşturup devam et.
- Test etmek için webte çalışacak şekilde olmalı. Direkt bir masaüstü uygulması değil bilgisayarlarda tarayıcı tabanlı Prograssive Web App şeklinde, mobilde ise cross-platform desteği ile eklensin. 
