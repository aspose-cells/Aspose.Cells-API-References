---
title: Axis.AxisLine
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Gets the appearance of an Axis
type: docs
url: /net/aspose.cells.charts/axis/axisline/
---
## Axis.AxisLine property

Gets the appearance of an Axis.

```csharp
public Line AxisLine { get; }
```

### Examples

```csharp
// Called: charttest.ValueAxis.AxisLine.Color = Color.BlueViolet;
[Test]
        public void Property_AxisLine()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet56882.xlsx");
            Worksheet sheettest = workbook.Worksheets[0];
            Chart charttest = sheettest.Charts[0];
            charttest.CategoryAxis.AxisLine.Color = Color.BlueViolet;
            charttest.ValueAxis.AxisLine.Color = Color.BlueViolet;
            charttest.CategoryAxis.Title.Font.Color = Color.BlueViolet;
            Assert.IsTrue(Util.CompareColor(Color.BlueViolet, charttest.CategoryAxis.AxisLine.Color));
        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


