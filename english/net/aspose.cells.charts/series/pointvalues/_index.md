---
title: Series.PointValues
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents the actual values that are used to plot every point in the chart. corresponding to Values When Series.Values is a link you can use this attribute to get specific data
type: docs
url: /net/aspose.cells.charts/series/pointvalues/
---
## Series.PointValues property

Represents the actual values that are used to plot every point in the chart. corresponding to [`Values`](../values/) When Series.Values is a link, you can use this attribute to get specific data.

```csharp

[C#]

Workbook workbook = new Workbook("YourFilePathName");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
// Values could be like "[External.xlsx]Sheet1!$A$1:$A$6", 
string Values = chart.NSeries[0].Values;
// But when you can't get point values from "[External.xlsx]Sheet1!$A$1:$A$6", 
// For example, "External.xlsx" does not exist, then you can use PointValues,
// It will return the values actually displayed in the Excel interface in the form of an array.
ChartDataValue[] v1 = chart.NSeries[0].PointValues;

```

```csharp
public ChartDataValue[] PointValues { get; }
```

### Remarks

For user's convenience, this property provides the actual values corresponding to the data defined by [`Values`](../values/).

### See Also

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


