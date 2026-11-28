---
title: "WorkbookRender.WorkbookRender"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookRender yapıcı. WorkbookRender'ın yapısı."
type: docs
url: /tr/net/aspose.cells.rendering/workbookrender/workbookrender/
---
## WorkbookRender constructor

WorkbookRender'in yapısı

```csharp
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| çalışma kitabı | Çalışma Kitabı | Hangi çalışma kitabının render edileceğini belirt. |
| seçenekler | ImageOrPrintOptions | ImageOrPrintOptions, çıktı görüntüsünün bazı özelliklerini içerir |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodctorWithWorkbookImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Görüntü/baskı seçenekleri oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Çalışma kitabı render'ı oluştur
            WorkbookRender renderer = new WorkbookRender(workbook, options);
            
            // Sayfa sayısını çıktı olarak ver
            Console.WriteLine("Total pages: " + renderer.PageCount);
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


