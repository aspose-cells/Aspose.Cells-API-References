---
title: DisplayUnitLabel.Text
second_title: Aspose.Cells for .NET API Reference
description: DisplayUnitLabel property. Gets or sets the text of display unit label
type: docs
url: /net/aspose.cells.charts/displayunitlabel/text/
---
## DisplayUnitLabel.Text property

Gets or sets the text of display unit label.

```csharp
public override string Text { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.ValueAxis.DisplayUnitLabel.Text, "百", "DisplayUnitLabel");
public void DisplayUnitLabel_Property_Text()
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

* class [DisplayUnitLabel](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


