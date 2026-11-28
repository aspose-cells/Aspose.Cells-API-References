---
title: "PageSetup.SetFirstPageFooter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup yöntemi. Bir Excel dosyasının ilk sayfa altbilgisini biçimlendiren bir betik ayarlar."
type: docs
url: /tr/net/aspose.cells/pagesetup/setfirstpagefooter/
---
## PageSetup.SetFirstPageFooter method

Excel dosyasının ilk sayfa alt bilgisini biçimlendiren bir betiği ayarlar.

```csharp
public void SetFirstPageFooter(int section, string footerScript)
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
    public class PageSetupMethodSetFirstPageFooterWithInt32StringDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // PageSetup nesnesini al
            PageSetup pageSetup = worksheet.PageSetup;
            
            // İlk sayfa için farklı başlık/altbilgiler ayarla
            pageSetup.IsHFDiffFirst = true;
            
            // Bölüm indeksi ve metinle ilk sayfa altbilgisini ayarla
            pageSetup.SetFirstPageFooter(0, "First Page Footer Text");
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            Console.WriteLine("First page footer set successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


