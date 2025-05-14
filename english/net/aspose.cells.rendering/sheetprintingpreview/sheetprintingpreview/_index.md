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
// Called: SheetPrintingPreview srp = new SheetPrintingPreview(wb.Worksheets[0], new ImageOrPrintOptions());
public void SheetPrintingPreview_Constructor()
{
    Workbook wb = new Workbook(Constants.TemplatePath + "example.xlsx");

    PageSetup pageSetup = wb.Worksheets[0].PageSetup;
    pageSetup.PrintArea = "1:59";
    pageSetup.SetFitToPages(0, 1);

    SheetRender sr = new SheetRender(wb.Worksheets[0], new ImageOrPrintOptions());
    int zoom = (int)(sr.PageScale * 100 + 0.5);
    Assert.AreEqual(64, zoom);

    pageSetup.Zoom = zoom;
    pageSetup.PrintArea = null;
    SheetPrintingPreview srp = new SheetPrintingPreview(wb.Worksheets[0], new ImageOrPrintOptions());
    Assert.AreEqual(6, srp.EvaluatedPageCount);
}
```

### See Also

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


