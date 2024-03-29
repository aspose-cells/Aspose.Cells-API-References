---
title: SetFooter
second_title: Aspose.Cells for .NET API Referansı
description: Bir Excel dosyasının alt bilgisini biçimlendiren bir komut dosyası ayarlar.
type: docs
weight: 600
url: /tr/net/aspose.cells/pagesetup/setfooter/
---
## PageSetup.SetFooter method

Bir Excel dosyasının alt bilgisini biçimlendiren bir komut dosyası ayarlar.

```csharp
public void SetFooter(int section, string footerScript)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| section | Int32 | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |
| footerScript | String | Altbilgi biçimi komut dosyası. |

### Notlar

Komut dosyası komutları:

**Emretmek**

**Tanım**

&amp;P

Geçerli sayfa numarası

&amp;N

Sayfa sayısı

&amp;D

Geçerli tarih

&amp;T

Şimdiki zaman

&amp;A

Sayfa adı

&amp;F

Yolu olmayan dosya adı

&amp;"&lt;Yazı TipiAdı&gt;"

Yazı tipi adı, örneğin: &amp;"Arial"

&amp;"&lt;FontName&gt;, &lt;FontStyle&gt;"

Yazı tipi adı ve yazı tipi stili, örneğin: &amp;"Arial,Kalın"

&amp;&lt;Yazı TipiBoyutu&gt;

Yazı Boyutu. Bu komutun ardından başlıkta yazdırılacak düz bir sayı geliyorsa, yazı tipi yüksekliğinden bir boşluk karakteri ile ayrılacaktır.

&amp;K&lt;RRGGBB&gt;

Yazı tipi rengi, örneğin(KIRMIZI): &amp;KFF0000

&amp;G

Resim komut dosyası

Örneğin: "&amp;Arial,Bold&amp;8Footer Note"

### Ayrıca bakınız

* class [PageSetup](../../pagesetup)
* ad alanı [Aspose.Cells](../../pagesetup)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
