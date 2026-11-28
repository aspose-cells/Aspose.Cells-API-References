---
title: "PageSetup.SetEvenFooter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup yöntemi. Excel dosyasının çift sayfa altbilgisini biçimlendiren bir betik ayarlar. Yalnızca IsHFDiffOddEven true olduğunda Excel 2007'de etkili olur"
type: docs
url: /tr/net/aspose.cells/pagesetup/setevenfooter/
---
## PageSetup.SetEvenFooter method

Excel dosyasının çift sayfa alt bilgisini biçimlendiren bir betiği ayarlar. Yalnızca IsHFDiffOddEven doğru olduğunda Excel 2007'de etkili olur.

```csharp
public void SetEvenFooter(int section, string footerScript)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bölüm | Int32 | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |
| footerScript | String | Altbilgi biçimlendirme betiği. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetEvenFooterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // İlk ve çift sayfalar için farklı üstbilgi/altbilgileri etkinleştir
            pageSetup.IsHFDiffFirst = true;
            pageSetup.IsHFDiffOddEven = true;

            // Farklı altbilgi türlerini ayarla
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            pageSetup.SetFooter(0, "Odd Page Footer");
            pageSetup.SetFirstPageFooter(0, "First Page Footer");

            // Çalışma kitabını kaydedin
            workbook.Save("PageSetup_SetEvenFooter_Example.xlsx");

            Console.WriteLine("Workbook saved with even page footer set successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


