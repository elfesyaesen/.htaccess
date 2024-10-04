### ** Htaccess Dosyasının Açıklaması:**

* **Seçenek 1:** RESTful API için temel .htaccess yapılandırması. Temiz URL'ler, güvenlik başlıkları ve yönlendirme kuralları içerir.
* **Seçenek 2:** Apache sunucusu için güvenlik ve performans iyileştirmeleri sağlayan .htaccess dosyası. Temiz URL'ler, yönlendirmeler ve güvenlik başlıkları içerir.

```
Bu .htaccess dosyası, bir RESTful API için özel olarak tasarlanmıştır ve aşağıdaki özellikleri içerir:

* **Temiz URL'ler:** Çirkin URL'leri daha okunaklı hale getirerek SEO'yu iyileştirir ve kullanıcı deneyimini artırır.
* **Güvenlik Başlıkları:** XSS ve diğer güvenlik açıklarına karşı koruma sağlar.
* **Yönlendirme Kuralları:** Tüm istekleri tek bir giriş noktasına yönlendirerek uygulamanın yapısını basitleştirir.
* **Performans Optimizasyonu:** Gereksiz dosya listelemelerini engeller ve sunucu kaynaklarını daha verimli kullanır.

**Ana Özellikler:**

* Trailing slash'ları kaldırır
* Tüm istekleri index.php'ye yönlendirir
* Directory listing'i devre dışı bırakır
* Güvenlik başlıkları ekler (No-Referrer, X-Content-Type-Options, Permissions-Policy)

**Kullanım:**

1. Bu dosyayı projenizin kök dizinine yerleştirin.
2. Apache sunucunuzda mod_rewrite ve mod_headers modüllerinin aktif olduğundan emin olun.
3. RewriteBase direktifi ile API'nizin temel URL'sini belirtin.

**Dikkat:**

* Options +FollowSymlinks satırı bazı durumlarda sorunlara neden olabilir. Gerekirse bu satırı yorum satırı haline getirin.

**Ek Bilgiler:**

* **mod_rewrite:** Apache'nin URL'leri yeniden yazma özelliğini sağlayan modülüdür.
* **mod_headers:** Apache'ye HTTP başlıkları ekleme özelliği kazandıran modüldür.
* **XSS:** Cross-site scripting, web sitelerine kötü amaçlı kod enjekte etme yöntemi.
* **FLOC:** Federated Learning of Cohorts, Google'ın kullanıcıları takip etmek için kullandığı bir teknolojidir.

**Bu .htaccess dosyasını kullanarak API'niz için daha güvenli ve performanslı bir ortam oluşturabilirsiniz.**
```

