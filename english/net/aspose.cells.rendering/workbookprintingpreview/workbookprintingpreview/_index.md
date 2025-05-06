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
// Called: WorkbookPrintingPreview wp = new WorkbookPrintingPreview(wb, new ImageOrPrintOptions());
[Test]
        public void WorkbookPrintingPreview_Constructor()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSJAVA-45829.xlsx&quot;);

            WorkbookPrintingPreview wp = new WorkbookPrintingPreview(wb, new ImageOrPrintOptions());
            Assert.AreEqual(114, wp.EvaluatedPageCount);
        }
```

### See Also

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


