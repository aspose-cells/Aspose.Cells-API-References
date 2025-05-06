---
title: Axis.CrossAt
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents the point on the value axis where the category axis crosses it
type: docs
url: /net/aspose.cells.charts/axis/crossat/
---
## Axis.CrossAt property

Represents the point on the value axis where the category axis crosses it.

```csharp
public double CrossAt { get; set; }
```

### Remarks

The number should be a integer when it applies to category axis. And the value must be between 1 and 31999.

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Charts[0].CategoryAxis.CrossAt, 0.65);
[Test]
        public void Property_CrossAt()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;TestTemplate2.xls&quot;);

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

            workbook.Save(Constants.destPath + &quot;Scatter_XCrossAt.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;Scatter_XCrossAt.xls&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Charts[0].CategoryAxis.CrossAt, 0.65);
        }
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


