# 📘 Proje Dokümantasyonu: Flask ile Kitap Okuma ve Satın Alma Uygulaması

Bu dokümantasyon, Flask kullanarak oluşturduğunuz kitap okuma ve satın alma uygulamanızın ayrıntılı açıklamalarını içermektedir.

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

## 🧐 İncelikler

Projenin önemli incelikleri ve kullanılan teknolojiler:

- Flask: Web uygulaması oluşturmak için kullanılan Python web çerçevesi.
- Flask-Login: Kullanıcı oturumu yönetimi için kullanılan Flask eklentisi.
- requests: API çağrıları yapmak için kullanılan Python modülü.
- smtplib ve email: E-posta doğrulama işlemleri için kullanılan Python modülleri.
- HTML ve CSS: Kullanıcı arayüzünü oluşturmak için kullanılan temel web teknolojileri.

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

Bu dokümantasyon, Flask ile geliştirilen kitap okuma ve satın alma uygulamanızın temel işleyişini ve ayrıntılarını açıklamaktadır. Uygulamanın geliştirilmesi ve özelleştirilmesi için bu dokümantasyonu kullanabilirsiniz. Başarılar dileriz! 👏📚
