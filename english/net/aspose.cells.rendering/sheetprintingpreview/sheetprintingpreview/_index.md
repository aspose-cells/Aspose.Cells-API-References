---
title: SheetPrintingPreview.SheetPrintingPreview
second_title: Aspose.Cells for .NET API Reference
description: SheetPrintingPreview constructor. The construct of SheetPrintingPreview
type: docs
url: /net/aspose.cells.rendering/sheetprintingpreview/sheetprintingpreview/
---
## SheetPrintingPreview constructor

The construct of SheetPrintingPreview

```csharp
public SheetPrintingPreview(Worksheet sheet, ImageOrPrintOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sheet | Worksheet | Indicate which spreadsheet to be printed. |
| options | ImageOrPrintOptions | ImageOrPrintOptions contains some property of output |

### Examples

```csharp
// Called: SheetPrintingPreview sheetPrintingPreview = new SheetPrintingPreview(worksheet, options);
public static void SheetPrintingPreview_Constructor()
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
```

### See Also

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


