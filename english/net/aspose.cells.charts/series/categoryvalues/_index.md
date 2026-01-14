---
title: Series.CategoryValues
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets the actual category values that are used to plot every point of this series in the chart
type: docs
url: /net/aspose.cells.charts/series/categoryvalues/
---
## Series.CategoryValues property

Gets the actual category values that are used to plot every point of this series in the chart.

```csharp
public ChartDataValue[][] CategoryValues { get; }
```

### Remarks

This property provides one convenient way to get the actual values corresponding to the data defined by [`XValues`](../xvalues/), especially when the specified data source is external link, formula, ...etc.

### Examples

```csharp
//Demo to show one case that requires this property:
[C#]

//Standalone example
Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
string XValues = chart.NSeries[0].XValues;
// XValues may be like "[External.xlsx]Sheet1!$B$2:$C$6" which is complicated
// for user to get the actual values(the values may be linked to another workbook,
// or cached in current workbook). Here you can use CategoryValues property
// to get the category values actually displayed in the Excel interface
// in the form of a two-dimensional array.
ChartDataValue[][] v1 = chart.NSeries[0].CategoryValues;

```

### See Also

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


