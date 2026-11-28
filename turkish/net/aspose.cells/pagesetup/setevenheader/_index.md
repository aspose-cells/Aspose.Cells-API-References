---
title: "PageSetup.SetEvenHeader"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup yöntemi. Excel dosyasının çift sayfa üstbilgisini biçimlendiren bir betik ayarlar. Yalnızca IsHFDiffOddEven true olduğunda Excel 2007'de etkilidir"
type: docs
url: /tr/net/aspose.cells/pagesetup/setevenheader/
---
## PageSetup.SetEvenHeader method

Excel dosyasının çift sayfa üst bilgisini biçimlendiren bir betiği ayarlar. Yalnızca IsHFDiffOddEven doğru olduğunda Excel 2007'de etkili olur.

```csharp
public void SetEvenHeader(int section, string headerScript)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bölüm | Int32 | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |
| headerScript | String | Başlık biçimlendirme betiği. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetEvenHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Tek ve çift sayfalar için farklı üstbilgi/altbilgi etkinleştir
            pageSetup.IsHFDiffOddEven = true;

            // Bölüm indeksi ve metin ile çift sayfa üstbilgisini ayarlayın
            pageSetup.SetEvenHeader(1, "Even Page Header - Center Section");
            pageSetup.SetEvenHeader(0, "Even Page Header - Left Section");
            pageSetup.SetEvenHeader(2, "Even Page Header - Right Section");

            // Çalışma kitabını kaydedin
            workbook.Save("PageSetup_SetEvenHeaderExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


