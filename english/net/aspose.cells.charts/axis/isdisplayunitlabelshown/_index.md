---
title: Axis.IsDisplayUnitLabelShown
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents if the display unit label is shown on the specified axis
type: docs
url: /net/aspose.cells.charts/axis/isdisplayunitlabelshown/
---
## Axis.IsDisplayUnitLabelShown property

Represents if the display unit label is shown on the specified axis.

```csharp
public bool IsDisplayUnitLabelShown { get; set; }
```

### Remarks

The default value is True.

### Examples

```csharp
// Called: chart.ValueAxis.IsDisplayUnitLabelShown = true;
[Test]
        public void Property_IsDisplayUnitLabelShown()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 10, 2, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            int seriesIndex = chart.NSeries.Add(&quot;{10,20,30,40}&quot;, true);
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            Assert.AreEqual(chart.ValueAxis.DisplayUnitLabel.Text, &quot;Hundreds&quot;, &quot;DisplayUnitLabel&quot;);
            wb.Settings.GlobalizationSettings.ChartSettings = new TestChartGlobalizationSetttings();
            Assert.AreEqual(chart.ValueAxis.DisplayUnitLabel.Text, &quot;百&quot;, &quot;DisplayUnitLabel&quot;);
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            Assert.AreEqual(chart.ValueAxis.DisplayUnitLabel.Text, &quot;千&quot;, &quot;DisplayUnitLabel&quot;);
        }
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


