---
title: Line.Color
second_title: Aspose.Cells for .NET API Reference
description: Line property. Represents the Color of the line
type: docs
url: /net/aspose.cells.drawing/line/color/
---
## Line.Color property

Represents the Color of the line.

```csharp
public Color Color { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(Util.CompareColor(Color.BlueViolet, charttest.CategoryAxis.AxisLine.Color));
[Test]
        public void Property_Color()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet56882.xlsx&quot;);
            Worksheet sheettest = workbook.Worksheets[0];
            Chart charttest = sheettest.Charts[0];
            charttest.CategoryAxis.AxisLine.Color = Color.BlueViolet;
            charttest.ValueAxis.AxisLine.Color = Color.BlueViolet;
            charttest.CategoryAxis.Title.Font.Color = Color.BlueViolet;
            Assert.IsTrue(Util.CompareColor(Color.BlueViolet, charttest.CategoryAxis.AxisLine.Color));
        }
```

### See Also

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


