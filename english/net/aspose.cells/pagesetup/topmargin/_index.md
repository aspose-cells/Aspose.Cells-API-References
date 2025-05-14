---
title: PageSetup.TopMargin
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the size of the top margin in unit of centimeters
type: docs
url: /net/aspose.cells/pagesetup/topmargin/
---
## PageSetup.TopMargin property

Represents the size of the top margin, in unit of centimeters.

```csharp
public double TopMargin { get; set; }
```

### Examples

```csharp
// Called: pgSetup.TopMargin = 0.04;
public void PageSetup_Property_TopMargin()
{
    Workbook wb = new Workbook(Constants.TemplatePath + "example.xlsx");
    Worksheet sheet = wb.Worksheets["Rendering"];
    Aspose.Cells.Range range = sheet.Workbook.Worksheets.GetRangeByName("ImageRange");

    PageSetup pgSetup = sheet.PageSetup;
    pgSetup.PrintArea = range.Address;
    pgSetup.LeftMargin = 0.04;
    pgSetup.TopMargin = 0.04;
    pgSetup.RightMargin = 0.04;
    pgSetup.BottomMargin = 0.04;
    var options = new ImageOrPrintOptions();
    options.ImageType = Aspose.Cells.Drawing.ImageType.Emf;
    options.OnlyArea = true;
    options.OnePagePerSheet = true;

    MemoryStream ms = new MemoryStream();
    SheetRender sr1 = new SheetRender(sheet, options);
    sr1.ToImage(0, ms);
    int originLength = ms.ToArray().Length;

    ms = new MemoryStream();
    options.IsOptimized = true;
    SheetRender sr2= new SheetRender(sheet, options);
    sr2.ToImage(0, ms);
    int optimizedLength = ms.ToArray().Length;

    Assert.IsTrue(optimizedLength < originLength);
}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


