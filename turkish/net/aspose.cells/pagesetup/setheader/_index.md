---
title: "PageSetup.SetHeader"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup yöntemi. Excel dosyasının başlığını biçimlendiren bir betik ayarlar"
type: docs
url: /tr/net/aspose.cells/pagesetup/setheader/
---
## PageSetup.SetHeader method

Excel dosyasının üstbilgisini biçimlendiren bir betik ayarlar.

```csharp
public void SetHeader(int section, string headerScript)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bölüm | Int32 | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |
| headerScript | String | Başlık biçimlendirme betiği. |

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

Örneğin: "&amp;Arial,Bold&amp;8Header Note"

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Farklı başlık bölümlerini çeşitli komutlarla ayarlayın
            pageSetup.SetHeader(0, "&F"); // Left section - File name
            pageSetup.SetHeader(1, "Page &P of &N"); // Center section - Page numbering
            pageSetup.SetHeader(2, "&D"); // Right section - Date

            workbook.Save("PageSetup_SetHeader_Example.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


