---
title: "Sınıf WorkbookPrintingPreview"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.WorkbookPrintingPreview sınıfı. Çalışma kitabı baskı önizlemesi"
type: docs
url: /tr/net/aspose.cells.rendering/workbookprintingpreview/
---
## WorkbookPrintingPreview class

Çalışma kitabı yazdırma önizlemesi.

```csharp
public class WorkbookPrintingPreview
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [WorkbookPrintingPreview](workbookprintingpreview/)(Workbook, ImageOrPrintOptions) | WorkbookPrintingPreview yapısı |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [EvaluatedPageCount](../../aspose.cells.rendering/workbookprintingpreview/evaluatedpagecount/) { get; } | Bu çalışma kitabının toplam sayfa sayısını değerlendirin |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class WorkbookPrintingPreviewDemo
    {
        public static void WorkbookPrintingPreviewExample()
        {
            // Mevcut bir çalışma kitabını yükleyin
            Workbook workbook = new Workbook("WorkbookPrintingPreviewExample_original.xlsx");

            // ImageOrPrintOptions bir örnek oluşturun
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // WorkbookPrintingPreview örneği oluşturun
            WorkbookPrintingPreview workbookPrintingPreview = new WorkbookPrintingPreview(workbook, options);

            // Çalışma kitabının toplam sayfa sayısını değerlendirin
            int pageCount = workbookPrintingPreview.EvaluatedPageCount;

            // Değerlendirilen sayfa sayısını yazdırın
            Console.WriteLine("Total Page Count: " + pageCount);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


