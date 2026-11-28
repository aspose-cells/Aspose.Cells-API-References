---
title: "PageSetup.GetFirstPageFooter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup yöntemi. Excel dosyasının ilk sayfa altbilgisini biçimlendiren bir betik alır"
type: docs
url: /tr/net/aspose.cells/pagesetup/getfirstpagefooter/
---
## PageSetup.GetFirstPageFooter method

Excel dosyasının ilk sayfa alt bilgisini biçimlendiren bir betiği alır.

```csharp
public string GetFirstPageFooter(int section)
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
    public class PageSetupMethodGetFirstPageFooterWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İlk sayfa altbilgisini ayarla
            worksheet.PageSetup.SetFirstPageFooter(1, "First Page Footer");

            // İlk sayfa altbilgisini al ve yazdır
            string footer = worksheet.PageSetup.GetFirstPageFooter(1);
            Console.WriteLine("First Page Footer: " + footer);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


