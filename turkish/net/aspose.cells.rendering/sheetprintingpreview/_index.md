---
title: "Class SheetPrintingPreview"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.SheetPrintingPreview sınıfı. Çalışma sayfası yazdırma önizlemesi"
type: docs
url: /tr/net/aspose.cells.rendering/sheetprintingpreview/
---
## SheetPrintingPreview class

Çalışma sayfası yazdırma önizlemesi.

```csharp
public class SheetPrintingPreview
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [SheetPrintingPreview](sheetprintingpreview/)(Worksheet, ImageOrPrintOptions) | SheetPrintingPreview yapısı |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [EvaluatedPageCount](../../aspose.cells.rendering/sheetprintingpreview/evaluatedpagecount/) { get; } | Bu çalışma sayfasının toplam sayfa sayısını değerlendirin |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetPrintingPreviewDemo
    {
        public static void SheetPrintingPreviewExample()
        {
            // Mevcut bir çalışma kitabını yükleyin
            Workbook workbook = new Workbook("SheetPrintingPreviewDemo_original.xlsx");

            // İlk çalışma sayfasını al
            Worksheet worksheet = workbook.Worksheets[0];

            // ImageOrPrintOptions bir örnek oluşturun
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // SheetPrintingPreview bir örnek oluşturun
            SheetPrintingPreview sheetPrintingPreview = new SheetPrintingPreview(worksheet, options);

            // Çalışma sayfasının toplam sayfa sayısını değerlendirin ve yazdırın
            Console.WriteLine("Total Page Count: " + sheetPrintingPreview.EvaluatedPageCount);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


