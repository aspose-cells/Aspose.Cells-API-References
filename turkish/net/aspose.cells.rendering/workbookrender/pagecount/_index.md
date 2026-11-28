---
title: "WorkbookRender.PageCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookRender özelliği. Çalışma kitabının toplam sayfa sayısını alır."
type: docs
url: /tr/net/aspose.cells.rendering/workbookrender/pagecount/
---
## WorkbookRender.PageCount property

Çalışma kitabının toplam sayfa sayısını alır.

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
    public class WorkbookRenderPropertyPageCountDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Page 1 Content");
            
            // İkinci bir çalışma sayfası ekle
            workbook.Worksheets.Add();
            worksheet = workbook.Worksheets[1];
            worksheet.Cells["A1"].PutValue("Page 2 Content");

            // Render seçenekleri ve çalışma kitabı render'ı oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true
            };
            
            WorkbookRender renderer = new WorkbookRender(workbook, options);

            // PageCount kullanımını göster
            Console.WriteLine($"Total pages to render: {renderer.PageCount}");
            
            // Her sayfayı görüntüye render et
            for (int i = 0; i < renderer.PageCount; i++)
            {
                string outputPath = $"Page_{i}.png";
                renderer.ToImage(i, outputPath);
                Console.WriteLine($"Rendered page {i+1} to {outputPath}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


