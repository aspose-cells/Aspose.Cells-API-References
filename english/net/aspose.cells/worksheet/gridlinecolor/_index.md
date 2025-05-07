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
[Test]
        public void Property_GridlineColor()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].GridlineColor = Color.Red;
            workbook.Save(Constants.destPath + "CellsNet58035.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet58035.xlsx");
            Assert.IsTrue(Util.CompareColor(Color.Red, workbook.Worksheets[0].GridlineColor));
            workbook.Save(Constants.destPath + "CellsNet58035.xls");
            workbook = new Workbook(Constants.destPath + "CellsNet58035.xls");
            Assert.IsTrue(Util.CompareColor(Color.Red, workbook.Worksheets[0].GridlineColor));
            workbook.Save(Constants.destPath + "CellsNet58035.xlsb");
            workbook = new Workbook(Constants.destPath + "CellsNet58035.xlsb");
            Assert.IsTrue(Util.CompareColor(Color.Red, workbook.Worksheets[0].GridlineColor));
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


