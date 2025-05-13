---
title: Cells.StandardHeight
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets or sets the default row height in this worksheet in unit of points
type: docs
url: /net/aspose.cells/cells/standardheight/
---
## Cells.StandardHeight property

Gets or sets the default row height in this worksheet, in unit of points.

```csharp
public double StandardHeight { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(wb.Worksheets[0].Cells.StandardHeight,15);
public void Cells_Property_StandardHeight()
{
    //test.CellsNet46949();
    LoadOptions options = new LoadOptions();
    options.AutoFitterOptions = new AutoFitterOptions();
    options.AutoFitterOptions.OnlyAuto = true;
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx", options);
    Assert.AreEqual(wb.Worksheets[0].Cells.StandardHeight,15);
    Workbook copy = new Workbook();
    copy.Copy(wb);
    Assert.AreEqual(copy.Worksheets[0].Cells.StandardHeight,15);
    wb.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


