# IDOR (Insecure Direct Object References) Nedir?

IDOR, yani "Güvensiz Doğrudan Nesne Referansları", bir kullanıcının, erişim izni olmadan başka bir kullanıcının verilerine ulaşabildiği bir güvenlik açığıdır.

# IDOR'un Olası Etkileri

Hesap devralma (Account Takeover)

Başka bir kullanıcının verilerini görüntüleme, değiştirme veya silme

Kritik, kamuya açık ya da özel verilere erişim
      biletler, faturalar, ödeme bilgileri, adresler, kimlik bilgileri vb.

# Gerçek Hayattan Basit Bir Örnek

Bir e-ticaret sitesinden kulaklık aldığımızı düşünelim. Sipariş sonrası sistem, faturayı görüntüleyebilmemiz için bir buton sunuyor. Bu butona tıkladığımızda tarayıcıda şu adrese yönlendiriliyoruz:

  https://keremticaret/faturagor/123


en basit haliyle Idor budur
