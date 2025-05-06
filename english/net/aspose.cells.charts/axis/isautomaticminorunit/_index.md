---
title: Axis.IsAutomaticMinorUnit
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Indicates whether the minor unit of the axis is automatically assigned
type: docs
url: /net/aspose.cells.charts/axis/isautomaticminorunit/
---
## Axis.IsAutomaticMinorUnit property

Indicates whether the minor unit of the axis is automatically assigned.

```csharp
public bool IsAutomaticMinorUnit { get; set; }
```

### Examples

```csharp
// Called: valueAxis.IsAutomaticMinorUnit = false;
public static void Property_IsAutomaticMinorUnit()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            // Adding a new worksheet to the Workbook object
            int sheetIndex = workbook.Worksheets.Add();
            // Obtaining the reference of the newly added worksheet by passing its sheet index
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Adding sample values to cells
            worksheet.Cells[&quot;A1&quot;].PutValue(50);
            worksheet.Cells[&quot;A2&quot;].PutValue(100);
            worksheet.Cells[&quot;A3&quot;].PutValue(150);
            worksheet.Cells[&quot;B1&quot;].PutValue(4);
            worksheet.Cells[&quot;B2&quot;].PutValue(20);
            worksheet.Cells[&quot;B3&quot;].PutValue(50);
            // Adding a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            // Accessing the instance of the newly added chart
            Chart chart = worksheet.Charts[chartIndex];
            // Adding NSeries (chart data source) to the chart ranging from &quot;A1&quot; cell to &quot;B3&quot;
            chart.NSeries.Add(&quot;A1:B3&quot;, true);

            // Accessing the value axis of the chart
            Axis valueAxis = chart.ValueAxis;
            // Setting properties of the value axis
            valueAxis.IsAutomaticMinValue = false;
            valueAxis.MinValue = 0;
            valueAxis.IsAutomaticMaxValue = false;
            valueAxis.MaxValue = 200;
            valueAxis.IsAutomaticMajorUnit = false;
            valueAxis.MajorUnit = 25;
            valueAxis.IsAutomaticMinorUnit = false;
            valueAxis.MinorUnit = 5;
            valueAxis.MajorTickMark = TickMarkType.Outside;
            valueAxis.MinorTickMark = TickMarkType.Inside;
            valueAxis.TickLabelPosition = TickLabelPositionType.NextToAxis;
            valueAxis.CrossAt = 0;
            valueAxis.CrossType = CrossType.Minimum;
            valueAxis.IsLogarithmic = false;
            valueAxis.IsPlotOrderReversed = false;
            valueAxis.AxisBetweenCategories = true;
            valueAxis.TickLabelSpacing = 1;
            valueAxis.IsAutoTickLabelSpacing = true;
            valueAxis.TickMarkSpacing = 1;
            valueAxis.DisplayUnit = DisplayUnitType.None;
            valueAxis.IsDisplayUnitLabelShown = false;
            valueAxis.CategoryType = CategoryType.AutomaticScale;
            valueAxis.BaseUnitScale = TimeUnit.Months;
            valueAxis.MajorUnitScale = TimeUnit.Months;
            valueAxis.MinorUnitScale = TimeUnit.Months;
            valueAxis.IsVisible = true;
            valueAxis.HasMultiLevelLabels = false;

            // Accessing the category axis of the chart
            Axis categoryAxis = chart.CategoryAxis;
            // Setting properties of the category axis
            categoryAxis.IsAutomaticMinValue = false;
            categoryAxis.MinValue = 0;
            categoryAxis.IsAutomaticMaxValue = false;
            categoryAxis.MaxValue = 3;
            categoryAxis.IsAutomaticMajorUnit = false;
            categoryAxis.MajorUnit = 1;
            categoryAxis.IsAutomaticMinorUnit = false;
            categoryAxis.MinorUnit = 0.5;
            categoryAxis.MajorTickMark = TickMarkType.Outside;
            categoryAxis.MinorTickMark = TickMarkType.Inside;
            categoryAxis.TickLabelPosition = TickLabelPositionType.NextToAxis;
            categoryAxis.CrossAt = 0;
            categoryAxis.CrossType = CrossType.Minimum;
            categoryAxis.IsLogarithmic = false;
            categoryAxis.IsPlotOrderReversed = false;
            categoryAxis.AxisBetweenCategories = true;
            categoryAxis.TickLabelSpacing = 1;
            categoryAxis.IsAutoTickLabelSpacing = true;
            categoryAxis.TickMarkSpacing = 1;
            categoryAxis.DisplayUnit = DisplayUnitType.None;
            categoryAxis.IsDisplayUnitLabelShown = false;
            categoryAxis.CategoryType = CategoryType.AutomaticScale;
            categoryAxis.BaseUnitScale = TimeUnit.Months;
            categoryAxis.MajorUnitScale = TimeUnit.Months;
            categoryAxis.MinorUnitScale = TimeUnit.Months;
            categoryAxis.IsVisible = true;
            categoryAxis.HasMultiLevelLabels = false;

            // Saving the Excel file
            workbook.Save(&quot;AxisExample.xlsx&quot;);
            workbook.Save(&quot;AxisExample.pdf&quot;);
        }
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


