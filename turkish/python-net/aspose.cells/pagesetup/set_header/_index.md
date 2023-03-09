---
title: set_header yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 200
url: /tr/python-net/aspose.cells/pagesetup/set_header/
is_root: false
---
##  set_header(section, header_script) {#int-str}
Bir Excel dosyasının başlığını biçimlendiren bir komut dosyası ayarlar.



```python
def set_header(self, section, header_script):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| section | int |0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm.|
| header_script | str | Başlık biçimi komut dosyası.|
###  Notlar

Komut dosyası komutları:

| Emretmek| Tanım|
| :- | :- |
| &P| Geçerli sayfa numarası|
| &N| Sayfa sayısı|
| &D| Geçerli tarih|
| &T| Şimdiki zaman|
| &A| Sayfa adı|
| &F| Yolsuz dosya adı|
| &"<FontName>"| Yazı tipi adı, örneğin: &"Arial"|
| &"<FontName>, <FontStyle>"| Yazı tipi adı ve yazı tipi stili, örneğin: &"Arial,Bold"|
| &<FontSize>| Yazı Boyutu. Bu komutun ardından başlıkta yazdırılacak düz bir sayı gelirse, yazı tipi yüksekliğinden bir boşluk karakteri ile ayrılır.|
| &K<RRGGBB>| Yazı tipi rengi, örneğin(KIRMIZI): &KFF0000|
| &G| Resim komut dosyası|

Örneğin: "&Arial,Bold&8Header Notu"


###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [PageSetup](/cells/tr/python-net/aspose.cells/pagesetup)
