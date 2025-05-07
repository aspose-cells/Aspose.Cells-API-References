---
title: Axis.DisplayUnitLabel
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents a unit label on an axis in the specified chart. Unit labels are useful for charting large values for example in the millions or billions
type: docs
url: /net/aspose.cells.charts/axis/displayunitlabel/
---
## Axis.DisplayUnitLabel property

Represents a unit label on an axis in the specified chart. Unit labels are useful for charting large values— for example, in the millions or billions.

```csharp
public DisplayUnitLabel DisplayUnitLabel { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.ValueAxis.DisplayUnitLabel.Text, "千", "DisplayUnitLabel");
[Test]
        public void Property_DisplayUnitLabel()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 10, 2, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            int seriesIndex = chart.NSeries.Add("{10,20,30,40}", true);
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            Assert.AreEqual(chart.ValueAxis.DisplayUnitLabel.Text, "Hundreds", "DisplayUnitLabel");
            wb.Settings.GlobalizationSettings.ChartSettings = new TestChartGlobalizationSetttings();
            Assert.AreEqual(chart.ValueAxis.DisplayUnitLabel.Text, "百", "DisplayUnitLabel");
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            Assert.AreEqual(chart.ValueAxis.DisplayUnitLabel.Text, "千", "DisplayUnitLabel");
        }
```

### See Also

* class [DisplayUnitLabel](../../displayunitlabel/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


