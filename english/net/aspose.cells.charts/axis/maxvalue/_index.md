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
// Called: Assert.AreEqual(100, chart.ValueAxis.MaxValue);
[Test]
        public void Property_MaxValue()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET48492.xlsx&quot;);
            workbook.Worksheets[0].Charts.Add(Aspose.Cells.Charts.ChartType.Bar100PercentStacked, 5, 5, 15, 15);
            workbook.Worksheets[0].Charts[0].SetChartDataRange(&quot;A1:C3&quot;, false);
            workbook.Worksheets[0].Charts[0].ValueAxis.MaxValue = 100;
            workbook.Worksheets[0].Charts[0].ValueAxis.MinValue = 25;
            workbook.Worksheets[0].Charts[0].ValueAxis.MajorUnit = 25;
            workbook.Worksheets[0].Charts[0].ValueAxis.MinorUnit = 1;
            workbook.Save(Constants.destPath + &quot;CELLSNET48492.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET48492.xlsx&quot;);
            Chart chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(100, chart.ValueAxis.MaxValue);
            Assert.AreEqual(25, chart.ValueAxis.MinValue);
            Assert.AreEqual(25, chart.ValueAxis.MajorUnit);
            Assert.AreEqual(1, chart.ValueAxis.MinorUnit);
        }
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


