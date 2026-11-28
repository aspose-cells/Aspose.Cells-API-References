---
title: "PageSetup.GetEvenFooter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup yöntemi. Excel dosyasının çift sayfa altbilgisini biçimlendiren bir betik alır"
type: docs
url: /tr/net/aspose.cells/pagesetup/getevenfooter/
---
## PageSetup.GetEvenFooter method

Excel dosyasının çift sayfa alt bilgisini biçimlendiren bir betiği alır.

```csharp
public string GetEvenFooter(int section)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bölüm | Int32 | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetEvenFooterWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Tek ve çift sayfalar için farklı üstbilgi/altbilgi etkinleştir
            pageSetup.IsHFDiffOddEven = true;
            
            // Çift sayfa altbilgisini ayarla
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            
            // Çift sayfa altbilgisini al ve göster
            string evenFooter = pageSetup.GetEvenFooter(0);
            Console.WriteLine("Even Footer: " + evenFooter);
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


