---
title: "SheetRender.SheetRender"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SheetRender yapıcı. SheetRender'in oluşturulması, worksheet ve ImageOrPrintOptions parametrelerini gerektirir."
type: docs
url: /tr/net/aspose.cells.rendering/sheetrender/sheetrender/
---
## SheetRender constructor

SheetRender'in yapısı, parametre olarak çalışma sayfası ve ImageOrPrintOptions gerektirir

```csharp
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| worksheet | Çalışma Sayfası | Render edilecek elektronik tabloyu belirtin. |
| seçenekler | ImageOrPrintOptions | ImageOrPrintOptions, çıktı görüntüsünün bazı özelliklerini içerir |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodCtorWithWorksheetImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluşturun ve bazı örnek veriler ekleyin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Görüntü/baskı seçenekleri oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;

            // Worksheet ve ImageOrPrintOptions ile SheetRender oluşturun
            SheetRender render = new SheetRender(worksheet, options);

            // Sayfa sayısını çıktı olarak ver
            Console.WriteLine("Page count: " + render.PageCount);

            // Render edilen görüntüyü kaydedin
            render.ToImage(0, "output.png");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


