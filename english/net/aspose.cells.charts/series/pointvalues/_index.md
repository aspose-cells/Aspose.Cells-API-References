---
title: Series.PointValues
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets the actual values that are used to plot every point of this series in the chart
type: docs
url: /net/aspose.cells.charts/series/pointvalues/
---
## Series.PointValues property

Gets the actual values that are used to plot every point of this series in the chart.

```csharp
public ChartDataValue[] PointValues { get; }
```

### Remarks

This property provides one convenient way to get the actual values corresponding to the data defined by [`Values`](../values/), especially when the specified data source is external link, formula, ...etc.

### Examples

```csharp
//Demo to show one case that requires this property:
[C#]

Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
string Values = chart.NSeries[0].Values;
// Values could be like "[External.xlsx]Sheet1!$A$1:$A$6" which is complicated
// for user to get the actual values(the values may be linked to another workbook,
// or cached in current workbook). Here you can use PointValues property
// to get the values actually displayed in the Excel interface
// in the form of an array.
ChartDataValue[] v1 = chart.NSeries[0].PointValues;

```

### See Also

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


