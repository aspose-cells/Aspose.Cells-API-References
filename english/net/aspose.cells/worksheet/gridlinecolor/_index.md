---
title: Worksheet.GridlineColor
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets and sets the color of gridline
type: docs
url: /net/aspose.cells/worksheet/gridlinecolor/
---
## Worksheet.GridlineColor property

Gets and sets the color of gridline

```csharp
public Color GridlineColor { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(Util.CompareColor(Color.Red, workbook.Worksheets[0].GridlineColor));
public void Worksheet_Property_GridlineColor()
{
    Workbook workbook = new Workbook();
    workbook.Worksheets[0].GridlineColor = Color.Red;
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.IsTrue(Util.CompareColor(Color.Red, workbook.Worksheets[0].GridlineColor));
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    Assert.IsTrue(Util.CompareColor(Color.Red, workbook.Worksheets[0].GridlineColor));
    workbook.Save(Constants.destPath + "example.xlsb");
    workbook = new Workbook(Constants.destPath + "example.xlsb");
    Assert.IsTrue(Util.CompareColor(Color.Red, workbook.Worksheets[0].GridlineColor));
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


