---
title: Class SheetPrintingPreview
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Rendering.SheetPrintingPreview class. Worksheet printing preview
type: docs
url: /net/aspose.cells.rendering/sheetprintingpreview/
---
## SheetPrintingPreview class

Worksheet printing preview.

```csharp
public class SheetPrintingPreview
```

## Constructors

| Name | Description |
| --- | --- |
| [SheetPrintingPreview](sheetprintingpreview/)(Worksheet, ImageOrPrintOptions) | The construct of SheetPrintingPreview |

## Properties

| Name | Description |
| --- | --- |
| [EvaluatedPageCount](../../aspose.cells.rendering/sheetprintingpreview/evaluatedpagecount/) { get; } | Evaluate the total page count of this worksheet |

### Examples

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
            // Load an existing workbook
            Workbook workbook = new Workbook("SheetPrintingPreviewDemo_original.xlsx");

            // Get the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Create an instance of ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Create an instance of SheetPrintingPreview
            SheetPrintingPreview sheetPrintingPreview = new SheetPrintingPreview(worksheet, options);

            // Evaluate and print the total page count of the worksheet
            Console.WriteLine("Total Page Count: " + sheetPrintingPreview.EvaluatedPageCount);
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


