---
title: WorkbookPrintingPreview.WorkbookPrintingPreview
second_title: Aspose.Cells for .NET API Reference
description: WorkbookPrintingPreview constructor. The construct of WorkbookPrintingPreview
type: docs
url: /net/aspose.cells.rendering/workbookprintingpreview/workbookprintingpreview/
---
## WorkbookPrintingPreview constructor

The construct of WorkbookPrintingPreview

```csharp
public WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | Indicate which workbook to be printed. |
| options | ImageOrPrintOptions | ImageOrPrintOptions contains some property of output |

### Examples

```csharp
// Called: WorkbookPrintingPreview workbookPrintingPreview = new WorkbookPrintingPreview(workbook, options);
public static void WorkbookPrintingPreview_Constructor()
        {
            // Load an existing workbook
            Workbook workbook = new Workbook("WorkbookPrintingPreviewExample_original.xlsx");

            // Create an instance of ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Create an instance of WorkbookPrintingPreview
            WorkbookPrintingPreview workbookPrintingPreview = new WorkbookPrintingPreview(workbook, options);

            // Evaluate the total page count of the workbook
            int pageCount = workbookPrintingPreview.EvaluatedPageCount;

            // Print the evaluated page count
            Console.WriteLine("Total Page Count: " + pageCount);
        }
```

### See Also

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


