---
title: Series.CategoryValues
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents the actual category values that are used in the chart. corresponding to XValues When Series.XValues is a link you can use this attribute to get specific data
type: docs
url: /net/aspose.cells.charts/series/categoryvalues/
---
## Series.CategoryValues property

Represents the actual category values that are used in the chart. corresponding to [`XValues`](../xvalues/) When Series.XValues is a link, you can use this attribute to get specific data.

```csharp

[C#]

Workbook workbook = new Workbook("YourFilePathName");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
// XValues could be like "[External.xlsx]Sheet1!$B$2:$C$6",
string XValues = chart.NSeries[0].XValues;
// But when you can't get category values from "[External.xlsx]Sheet1!$B$2:$C$6",
// For example, "External.xlsx" does not exist, then you can use CategoryValues,
// It will return the category values actually displayed in the Excel interface in the form of a two-dimensional array.
ChartDataValue[][] v1 = chart.NSeries[0].CategoryValues;

```

```csharp
public ChartDataValue[][] CategoryValues { get; }
```

### Remarks

For user's convenience, this property provides the actual values corresponding to the data defined by [`XValues`](../xvalues/).

### See Also

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


