---
title: "PageSetup.GetEvenHeader"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup yöntemi. Excel dosyasının çift başlığını biçimlendiren bir betik alır."
type: docs
url: /tr/net/aspose.cells/pagesetup/getevenheader/
---
## PageSetup.GetEvenHeader method

Excel dosyasının çift sayfa üst bilgisini biçimlendiren bir betiği alır.

```csharp
public string GetEvenHeader(int section)
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
    public class PageSetupMethodGetEvenHeaderWithInt32Demo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Tek ve çift sayfa başlıkları/altbilgileri farklı olmasını etkinleştir
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.IsHFDiffOddEven = true;
            
            // Çift sayfa başlığını ayarla
            pageSetup.SetEvenHeader(0, "&CEven Page Header Center");
            pageSetup.SetEvenHeader(1, "&LEven Page Header Left");
            pageSetup.SetEvenHeader(2, "&REven Page Header Right");
            
            // Çift sayfa başlıklarını al ve yazdır
            Console.WriteLine("Even Header Center: " + pageSetup.GetEvenHeader(0));
            Console.WriteLine("Even Header Left: " + pageSetup.GetEvenHeader(1));
            Console.WriteLine("Even Header Right: " + pageSetup.GetEvenHeader(2));
            
            // Çalışma kitabını kaydedin
            workbook.Save("PageSetup_GetEvenHeaderDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


