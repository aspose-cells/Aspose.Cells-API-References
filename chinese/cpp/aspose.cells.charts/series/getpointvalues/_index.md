---
title: Aspose::Cells::Charts::Series::GetPointValues method
linktitle: GetPointValues
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::Series::GetPointValues method. Gets the actual values that are used to plot every point of this series in the chart in C++.'
type: docs
weight: 2000
url: /zh/cpp/aspose.cells.charts/series/getpointvalues/
---
## Series::GetPointValues method


Gets the actual values that are used to plot every point of this series in the chart.

```cpp
Vector<ChartDataValue> Aspose::Cells::Charts::Series::GetPointValues()
```

## Remarks


This property provides one convenient way to get the actual values corresponding to the data defined by Series.Values, especially when the specified data source is external link, formula, ...etc. 

## Examples


```cpp
Aspose::Cells::Startup();
Workbook workbook(u"ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.GetWorksheets().Get(0);
Chart chart = worksheet.GetCharts().Get(0);
chart.Calculate();
U16String Values = chart.GetNSeries().Get(0).GetValues();
// Values 可能类似于 "[External.xlsx]Sheet1!$A$1:$A$6"，这比较复杂
// 供用户获取实际值（这些值可能链接到另一个工作簿，
// 或者缓存于当前工作簿）。此处可使用 PointValues 属性
// 获取在 Excel 界面实际显示的值
// 以数组的形式。
//Vector<ChartDataValue> v1 = chart.GetNSeries().Get(0).GetPointValues();
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [ChartDataValue](../../chartdatavalue/)
* Class [Series](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
