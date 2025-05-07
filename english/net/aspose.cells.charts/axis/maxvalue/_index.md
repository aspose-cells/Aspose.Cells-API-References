---
title: Axis.MaxValue
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents the maximum value on the value axis
type: docs
url: /net/aspose.cells.charts/axis/maxvalue/
---
## Axis.MaxValue property

Represents the maximum value on the value axis.

```csharp
public object MaxValue { get; set; }
```

### Remarks

The maxValue type only can be double or DateTime

### Examples

```csharp
// Called: chart.ValueAxis.MaxValue = 80;
[Test]
        public void Property_MaxValue()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "TestTemplate2.xls");

            Cells cells = workbook.Worksheets[1].Cells;
            Style style = workbook.CreateStyle();

            cells[0, 2].PutValue(0.6);
            cells[0, 3].PutValue(50);

            cells[1, 2].PutValue(0.7);
            cells[1, 3].PutValue(75.5);
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.CategoryAxis.MinValue = 0.4;
            chart.CategoryAxis.MaxValue = 0.8;
            chart.CategoryAxis.CrossAt = 0.65;

            chart.ValueAxis.MinValue = 40;
            chart.ValueAxis.MaxValue = 80;
            chart.ValueAxis.CrossAt = 63;

            workbook.Save(Constants.destPath + "Scatter_XCrossAt.xls");
            workbook = new Workbook(Constants.destPath + "Scatter_XCrossAt.xls");
            Assert.AreEqual(workbook.Worksheets[0].Charts[0].CategoryAxis.CrossAt, 0.65);
        }
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


