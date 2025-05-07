---
title: PageSetup.SetFitToPages
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Sets the number of pages the worksheet will be scaled to when its printed
type: docs
url: /net/aspose.cells/pagesetup/setfittopages/
---
## PageSetup.SetFitToPages method

Sets the number of pages the worksheet will be scaled to when it's printed.

```csharp
public void SetFitToPages(int wide, int tall)
```

| Parameter | Type | Description |
| --- | --- | --- |
| wide | Int32 | Pages wide. |
| tall | Int32 | Pages tall. |

### Examples

```csharp
// Called: pageSetup.SetFitToPages(0, 1);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook(Constants.TemplatePath + "CELLSNET-51864.xlsx");

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

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


