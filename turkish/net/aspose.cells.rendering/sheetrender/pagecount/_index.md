---
title: "SheetRender.PageCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SheetRender özelliği. Mevcut çalışma sayfasının toplam sayfa sayısını alır"
type: docs
url: /tr/net/aspose.cells.rendering/sheetrender/pagecount/
---
## SheetRender.PageCount property

Geçerli çalışma sayfasının toplam sayfa sayısını alır.

```csharp
public int PageCount { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderPropertyPageCountDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Mary");
            cells["B3"].PutValue(25);
            cells["A4"].PutValue("Peter");
            cells["B4"].PutValue(35);

            // Yazdırma için sayfa ayarlarını ayarlayın
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PrintArea = "A1:B4";
            pageSetup.FitToPagesTall = 1;
            pageSetup.FitToPagesWide = 1;

            // Varsayılan seçeneklerle SheetRender oluşturun
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            SheetRender render = new SheetRender(worksheet, options);

            // Sayfa sayısını görüntüleyin
            Console.WriteLine("Page Count: " + render.PageCount);

            // Birden çok sayfa zorlamak için sayfa ayarlarını değiştirin
            pageSetup.FitToPagesTall = 0;
            pageSetup.FitToPagesWide = 1;
            pageSetup.PrintArea = "A1:B100"; // Larger area than can fit on one page

            // Güncellenmiş sayfa sayısını almak için yeni SheetRender oluşturun
            SheetRender newRender = new SheetRender(worksheet, options);
            Console.WriteLine("Updated Page Count: " + newRender.PageCount);
        }
    }
}
```

### Ayrıca Bakınız

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


