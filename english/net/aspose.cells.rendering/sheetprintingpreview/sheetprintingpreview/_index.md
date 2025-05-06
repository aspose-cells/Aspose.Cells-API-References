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
// Called: SheetPrintingPreview sheetPw = new SheetPrintingPreview(wb.Worksheets[0], new ImageOrPrintOptions());
[Test]
        public void SheetPrintingPreview_Constructor()
        {
            Workbook wb = new Workbook(Constants.TemplatePath + &quot;CELLSPYTHONJAVA-99.xlsm&quot;);

            SheetPrintingPreview sheetPw = new SheetPrintingPreview(wb.Worksheets[0], new ImageOrPrintOptions());
            Assert.AreEqual(20, sheetPw.EvaluatedPageCount);
        }
```

### See Also

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


