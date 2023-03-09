---
title: set_footer yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 180
url: /tr/python-net/aspose.cells/pagesetup/set_footer/
is_root: false
---
##  set_footer(section, footer_script) {#int-str}
Bir Excel dosyasının altbilgisini biçimlendiren bir komut dosyası ayarlar.



```python
def set_footer(self, section, footer_script):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| section | int |0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm.|
| footer_script | str | Altbilgi biçimi komut dosyası.|
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

Örneğin: "&Arial,Bold&8Footer Note"


###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [PageSetup](/cells/tr/python-net/aspose.cells/pagesetup)
