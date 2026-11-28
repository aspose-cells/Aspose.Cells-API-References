---
title: "PageSetup.GetFooter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup yöntemi. Excel dosyasının altbilgisini biçimlendiren bir betik alır."
type: docs
url: /tr/net/aspose.cells/pagesetup/getfooter/
---
## PageSetup.GetFooter method

Excel dosyasının alt bilgisini biçimlendiren bir betiği alır.

```csharp
public string GetFooter(int section)
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
    public class PageSetupMethodGetFooterWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Farklı altbilgi bölümlerini ayarla
            worksheet.PageSetup.SetFooter(1, "odd");
            worksheet.PageSetup.SetFirstPageFooter(1, "first");
            worksheet.PageSetup.SetEvenFooter(1, "even");

            // Altbilgi bölümlerini al ve göster
            Console.WriteLine("First Page Footer: " + worksheet.PageSetup.GetFirstPageFooter(1));
            Console.WriteLine("Even Page Footer: " + worksheet.PageSetup.GetEvenFooter(1));
            Console.WriteLine("Odd Page Footer: " + worksheet.PageSetup.GetFooter(1));
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


