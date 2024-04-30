# ARK-ISTEGI-IPTAL-ETME

### ADIM 1

<p>- Facebook dilini Türkçe yap</p>
<p>- Tampermonkey eklentisi tarayıcınıza ekleyin</p>
<p>- Yeni Betik oluştura tıklayın</p>

![image](https://github.com/DenizKod/ARK-ISTEGI-IPTAL-ETME/assets/168285638/7e1b2696-803e-447a-ae3f-f7844a44d28f)

#### Aşağıdaki kodu betik oluşturma sayfasına yapıştırıp betiği kaydedin

```
// ==UserScript==
// @name         Facebook Arkadaşlık isteklerini iptal etme
// @namespace    http://tampermonkey.net/
// @version      0.1
// @description  Facebook Arkadaşlık isteklerini iptal etme
// @author       Deniz Kod
// @match        *://*.facebook.com/*
// @grant        none
// ==/UserScript==
(function() {
    'use strict';
    document.addEventListener('keydown', function(e) {
        // Scrollock tuşunun keyCode'u 145'tür
        if (e.keyCode === 145) {
            // Butonu seç
            var buton = document.querySelector('div[aria-label="İsteği İptal Et"][role="button"]');
            if (buton) {
                buton.click();
            }
        }
    });
})();
```

<p>- Sayfaya git : https://www.facebook.com/friends/requests </p>

![image](https://github.com/DenizKod/ARK-ISTEGI-IPTAL-ETME/assets/168285638/858ddd23-51d0-4348-9286-91cc2f1feaea)

<p>- Scrollock Tuşuna bas yada basılı tut. </p>

#### TEBRIKLER, ARTIK TÜM ARKADAŞLIK İSTEKLERİ İPTAL OLDU <3
