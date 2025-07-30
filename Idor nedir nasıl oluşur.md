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

Buradaki 123 sayısı, fatura numarasını temsil ediyor olabilir. Eğer bu sayıyı manuel olarak değiştirir ve örneğin 122 yaparsak:

      https://keremticaret/faturagor/122

bizim dışımızdaki başka bir kullanıcının faturasına erişebiliriz. Bu fatura içinde:

İsim-soyisim

Adres

Sipariş bilgileri

Ödeme detayları gibi kişisel ve hassas bilgiler yer alıyor olabilir.

Bu, açık bir IDOR (yetkisiz erişim) zafiyetidir. Sistem, erişim kontrolü yapmadığı için herkes herhangi bir fatura numarasını girerek başka kullanıcılara ait bilgilere ulaşabilir.


