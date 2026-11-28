---
title: "PageSetup.SetFooter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup yöntemi. Excel dosyasının altbilgisini biçimlendiren bir betik ayarlar"
type: docs
url: /tr/net/aspose.cells/pagesetup/setfooter/
---
## PageSetup.SetFooter method

Excel dosyasının altbilgisini biçimlendiren bir betik ayarlar.

```csharp
public void SetFooter(int section, string footerScript)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bölüm | Int32 | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |
| footerScript | String | Altbilgi biçimlendirme betiği. |

### Açıklamalar

Betik komutları:

| **Command** | **Description** |
| --- | --- |
| &amp;P | Geçerli sayfa numarası |
| &amp;N | Sayfa sayısı |
| &amp;D | Geçerli tarih |
| &amp;T | Geçerli zaman |
| &amp;A | Sayfa adı |
| &amp;F | Yol olmadan dosya adı |
| &amp;\"&lt;FontName&gt;\" | Yazı tipi adı, örneğin: &amp;\"Arial\" |
| &amp;\"&lt;FontName&gt;, &lt;FontStyle&gt;\" | Yazı tipi adı ve yazı tipi stili, örneğin: &amp;\"Arial,Bold\" |
| &amp;&lt;FontSize&gt; | Yazı tipi boyutu. Bu komut, başlıkta yazdırılacak düz bir sayı ile takip edilirse, yazı yüksekliğinden bir boşluk karakteri ile ayrılır. |
| &amp;K&lt;RRGGBB&gt; | Yazı tipi rengi, örneğin(KIRMIZI): &amp;KFF0000 |
| &amp;G | Görüntü betiği |

Örneğin: "&amp;Arial,Bold&amp;8Footer Note"

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFooterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.PageSetup.SetFooter(0, "Page &P");
            worksheet.PageSetup.SetFooter(1, "&D");
            worksheet.PageSetup.SetFooter(2, "&A");
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


