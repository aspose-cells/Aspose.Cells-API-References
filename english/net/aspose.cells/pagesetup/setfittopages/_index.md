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
            Workbook wb = new Workbook(Constants.TemplatePath + &quot;CELLSNET-52043.xlsx&quot;);

            PageSetup pageSetup = wb.Worksheets[0].PageSetup;
            pageSetup.PrintArea = &quot;1:59&quot;;
            pageSetup.SetFitToPages(0, 1);

            SheetRender sr = new SheetRender(wb.Worksheets[0], new ImageOrPrintOptions());
            int zoom = (int)(sr.PageScale * 100 + 0.5);
            Assert.AreEqual(53, zoom);
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


