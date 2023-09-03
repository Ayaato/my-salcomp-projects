# 📘 Proje Dokümantasyonu: Flask ile Kitap Okuma ve Satın Alma Uygulaması

Bu dokümantasyon, Flask kullanarak oluşturduğunuz kitap okuma ve satın alma uygulamanızın ayrıntılı açıklamalarını içermektedir.

*Önceden belirtmeliyim ki: bu sitenin tasarımı tamamen bana ait değildir, ancak arkauç yazılımı tamamen bana aittir.*

## 🎯 Proje Amacı

Bu proje, kullanıcıların çevrimiçi kitapları satın almasını veya okumasını sağlayan basit bir web uygulamasını hedeflemektedir. Kullanıcılar, bir e-posta adresi aracılığıyla giriş yapar, kitapları görüntüler ve satın alır veya okur. Projede aşağıdaki temel özellikler bulunmaktadır:

- Kullanıcı Girişi
- E-posta Doğrulama
- Kitapları Görüntüleme
- Kitap Satın Alma veya Okuma
- Tema ve Stil Seçenekleri

## 🚀 Nasıl Çalıştırılır

Projeyi yerel makinenizde çalıştırmak için aşağıdaki adımları izleyebilirsiniz:

1. Projeyi bilgisayarınıza klonlayın veya zip dosyasını indirin.

2. Python yüklü değilse [Python](https://www.python.org/downloads/) web sitesinden indirin ve yükleyin.

3. Gerekli bağımlılıkları kurmak için terminalde proje dizinine gidin ve aşağıdaki komutu çalıştırın:

   ```bash
   pip install -r requirements.txt
   ```

4. Proje dizinindeyken aşağıdaki komutu çalıştırarak Flask uygulamasını başlatın:

   ```bash
   python main.py
   ```

5. Tarayıcınızda [http://localhost:80](http://localhost:80) adresine gidin ve uygulamayı kullanmaya başlayın.

Elbette, kodların ana işlevlerini daha ayrıntılı bir şekilde açıklayan bir bölüm ekleyebilirim. İşte kodların ana işlevlerini açıklayan ek bir bölüm:

## 🔍 Kodların Ana İşlevleri

Proje içindeki Python kodlarının ana işlevleri şunlardır:

### `main.py` İşlevleri

1. **Kullanıcı Girişi ve Oturum Yönetimi**

   - `User` sınıfı, kullanıcıları temsil etmek için kullanılır.
   - `load_user` fonksiyonu, kullanıcıları ID'leriyle yüklemek için kullanılır.
   - `login_manager` ile oturum yönetimi sağlanır.

2. **E-posta Adreslerini API'den Getirme**

   - `get_emails` fonksiyonu, API'den müşteri e-posta adreslerini çeker ve `customer_emails` listesine depolar.

3. **Ana Sayfa (`/`)**

   - `main` fonksiyonu, ana sayfayı temsil eder ve `main.html` şablonunu döndürür.

4. **E-posta Doğrulama İşlemi**

   - `create_verification_code` fonksiyonu, rastgele bir doğrulama kodu oluşturur.
   - `send_code_to_mail` fonksiyonu, kullanıcıya e-posta ile doğrulama kodu gönderir.

5. **Kitapları Görüntüleme ve Yönlendirme**

   - `login` fonksiyonu, kullanıcının kitapları görüntülemesi için giriş yapmasını sağlar.
   - `check_verification` fonksiyonu, kullanıcının doğrulama kodunu kontrol eder ve kitapları yönlendirir.

6. **Kitap Sayfaları**

   - `firstbook` ve `secondbook` fonksiyonları, kullanıcının kitapları görüntülemesini sağlar.

### HTML Dosyaları İşlevleri

1. **`main.html`**: Ana sayfa tasarımını içerir. Kullanıcının kitapları görüntüleyebilmesi için bir kart tasarımı sunar.

2. **`login.html`**: Kullanıcının e-posta adresini girebileceği bir form sunar.

3. **`verification.html`**: Doğrulama kodunu girmek için bir form sunar.

4. **`firstbook.html` ve `secondbook.html`**: Kitap sayfalarının tasarımını içerir. Kullanıcıların kitapları okuyabilmesi için bir görünüm sunar.

5. **`error_page.html`**: Hataları ve uyarıları gösteren bir sayfa tasarımı sunar.

## 🧰 Teknolojiler ve Kütüphaneler

- **Flask**: Web uygulaması geliştirmek için kullanılan Python çerçevesi.
- **Flask-Login**: Kullanıcı oturumu yönetimi için kullanılan Flask eklentisi.
- **requests**: API çağrıları yapmak için kullanılan Python modülü.
- **smtplib ve email**: E-posta doğrulama işlemleri için kullanılan Python modülleri.
- **HTML ve CSS**: Kullanıcı arayüzünü oluşturmak için kullanılan temel web teknolojileri.

## 📁 Dosya Dizini

Proje dosya dizini aşağıdaki şekildedir:

```
- Bonus Project
    - static
        favicon.ico
        main.css
        pdf.css
        style.css
        pdf.js
        pdf.worker.js
    - templates
        error_page.html
        firstbook.html
        login.html
        main.html
        secondbook.html
        verification.html
    main.py
    README.md
```

## 📂 Dosya Açıklamaları

- `main.py`: Flask uygulamasının ana dosyasıdır. Kullanıcı girişi, e-posta doğrulama, kitap görüntüleme ve yönlendirme işlemlerini içerir.

- `static`: Stil dosyaları ve favicon gibi statik dosyaların bulunduğu klasördür.

- `templates`: Flask uygulamanızın HTML şablonlarını içeren klasördür.

## 🧑‍💻 Python Kodlarının İşlevleri

Proje içindeki Python kodları aşağıdaki işlevlere sahiptir:

- Kullanıcı girişi ve oturum yönetimi.
- E-posta doğrulama ve e-posta gönderme işlemleri.
- API kullanarak kitapları görüntüleme.
- Kullanıcının kitapları satın alma veya okuma işlemleri.

## 🌐 HTML Dosyaları

Projedeki HTML dosyaları, kullanıcı arayüzünün tasarlandığı ve Flask ile birleştirildiği dosyalardır. HTML dosyaları, kullanıcıların kitapları görüntülemesini ve işlemlerini gerçekleştirmesini sağlar.

---
