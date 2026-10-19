# cloudstream-domain-list

frukon eklentilerinin kullandığı güncel alan adları. Eklentiler `eklenti_domainleri.txt` dosyasını
açılışta çekip kendi adresini buradan okur; bir site taşınırsa eklentiyi yeniden derlemeden yalnızca
bu dosyadaki satırı değiştirmek yeterli.

Biçim: `|EklentiAdı:https://alanadi.com` (her satıra bir eklenti, sonda `/` yok).

`domain-checker.yml` her 45 dakikada bir adresleri açıp yönlendirmeleri takip eder, yeni adres
bulursa dosyayı kendisi günceller. `domain_blacklist.txt` içindeki alan adlarına yönlendirme olursa
mevcut adres korunur.
