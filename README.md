# Chatbot Uygulaması README Dosyası

## Açıklama
Bu Python uygulaması, basit bir chatbot simülasyonu içerir. Kullanıcının yazdığı mesajlara önceden tanımlanmış yanıtlar vererek etkileşim sağlar. Chatbot, kullanıcıyla temel bir sohbet deneyimi sunar.

## Özellikler
- Kullanıcı tarafından gönderilen belirli mesajlara yanıt verebilme.
- Rastgele yanıt seçimi ile daha dinamik bir sohbet deneyimi sağlama.
- Belirli komutlara uygun cevaplar döndürme.

## Kullanım
1. **Gerekli Ortam**: Uygulama, Python 3.x sürümünde çalışacak şekilde tasarlanmıştır. Ek bir kütüphane kurulumu gerekmez.
2. **Uygulamayı Çalıştırma**:
    - Kod dosyasını bir Python editörüne yapıştırın veya bir Python dosyası olarak kaydedin (örneğin, `chatbot.py`).
    - Terminal veya komut satırında dosyayı çalıştırın:
      ```
      python chatbot.py
      ```
3. **Chatbot ile Etkileşim**:
    - Program çalıştırıldığında, kullanıcıdan bir girdi bekler.
    - Kullanıcı bir mesaj girdiğinde, chatbot ilgili yanıtı verecektir.
    - Mesajların anahtar kelimelere uygun olması gerekir (örneğin, "merhaba", "nasılsın", "adın ne" gibi).
    - "görüşürüz" yazıldığında program sonlanır.

## Örnek Kullanım
**Giriş:**
```
merhaba
```
**Çıkış:**
```
Merhaba! Size nasıl yardımcı olabilirim?
```

**Giriş:**
```
nasılsın
```
**Çıkış:**
```
Ben robotum, her zaman iyiyim!
```

**Giriş:**
```
görüşürüz
```
**Çıkış:**
```
Hoşça kalın!
```

## Kod Yapısı
1. **Yanıtlar Sözlüğü (`responses`)**:
    - Kullanıcı mesajları ve chatbot yanıtlarını içerir.
    - Anahtar kelimeler, chatbot'un kullanıcıya yanıt verebilmesi için eşleştirilmiştir.
    - Her bir anahtar kelime birden fazla yanıt içerebilir ve bu yanıtlar rastgele seçilir.

2. **`chatbot()` Fonksiyonu**:
    - Sonsuz bir döngü ile çalışır.
    - Kullanıcıdan giriş alır ve bu girişe uygun yanıtı `responses` sözlüğünden seçer.
    - Eğer kullanıcı "görüşürüz" yazarsa, döngüyü sonlandırır ve programı kapatır.

## Geliştirme
Chatbot'u geliştirmek isterseniz, aşağıdaki adımları izleyebilirsiniz:
- **Yeni Mesaj ve Yanıtlar Ekleyin**: `responses` sözlüğüne yeni anahtar kelimeler ve bunlara uygun yanıtlar ekleyebilirsiniz.
- **Fonksiyonlar Ekleyin**: Daha karmaşık bir işlevsellik sağlamak için yeni fonksiyonlar oluşturabilirsiniz.
- **Hata Yönetimi**: Kullanıcının anlamlı bir yanıt alamadığı durumlar için "anlamadım" gibi varsayılan yanıtlar ekleyebilirsiniz.

## Önemli Notlar
- Chatbot sadece tanımlı anahtar kelimeler ile çalışır. Diğer mesajlara yanıt vermez.
- Geliştirilen bu uygulama temel bir simülasyon olup, gerçek bir yapay zeka içermemektedir.
