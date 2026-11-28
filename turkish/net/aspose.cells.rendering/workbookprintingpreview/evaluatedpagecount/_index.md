---
title: "WorkbookPrintingPreview.EvaluatedPageCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookPrintingPreview özelliği. Bu çalışma kitabının toplam sayfa sayısını değerlendirin"
type: docs
url: /tr/net/aspose.cells.rendering/workbookprintingpreview/evaluatedpagecount/
---
## WorkbookPrintingPreview.EvaluatedPageCount property

Bu çalışma kitabının toplam sayfa sayısını değerlendirin

```csharp
public int EvaluatedPageCount { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookPrintingPreviewPropertyEvaluatedPageCountDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına örnek veri ekle
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].PutValue("Row " + (i + 1));
            }

            // Yazdırma önizleme seçenekleri oluşturun
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Çalışma kitabı yazdırma önizlemesi oluşturun
            WorkbookPrintingPreview printingPreview = new WorkbookPrintingPreview(workbook, options);
            
            // Değerlendirilen sayfa sayısını alın ve görüntüleyin
            Console.WriteLine("Evaluated Page Count: " + printingPreview.EvaluatedPageCount);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


