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
            workbook.Save(Constants.destPath + &quot;CellsNet58035.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet58035.xlsx&quot;);
            Assert.IsTrue(Util.CompareColor(Color.Red, workbook.Worksheets[0].GridlineColor));
            workbook.Save(Constants.destPath + &quot;CellsNet58035.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet58035.xls&quot;);
            Assert.IsTrue(Util.CompareColor(Color.Red, workbook.Worksheets[0].GridlineColor));
            workbook.Save(Constants.destPath + &quot;CellsNet58035.xlsb&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet58035.xlsb&quot;);
            Assert.IsTrue(Util.CompareColor(Color.Red, workbook.Worksheets[0].GridlineColor));
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


