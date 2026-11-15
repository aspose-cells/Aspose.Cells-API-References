---
title: Aspose::Cells::Charts::Series::GetCategoryValues method
linktitle: GetCategoryValues
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::Series::GetCategoryValues method. Gets the actual category values that are used to plot every point of this series in the chart in C++.'
type: docs
weight: 2100
url: /ru/cpp/aspose.cells.charts/series/getcategoryvalues/
---
## Series::GetCategoryValues method


Gets the actual category values that are used to plot every point of this series in the chart.

```cpp
Vector<Vector<ChartDataValue>> Aspose::Cells::Charts::Series::GetCategoryValues()
```

## Remarks


This property provides one convenient way to get the actual values corresponding to the data defined by Series.XValues, especially when the specified data source is external link, formula, ...etc. 

## Examples


```cpp
Aspose::Cells::Startup();
Workbook workbook(u"ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.GetWorksheets().Get(0);
Chart chart = worksheet.GetCharts().Get(0);
chart.Calculate();
U16String XValues = chart.GetNSeries().Get(0).GetXValues();
// XValues могут выглядеть как "[External.xlsx]Sheet1!$B$2:$C$6", что сложно
// для получения пользователем фактических значений (значения могут быть связаны с другой книгой,
// или кэшированы в текущей книге). Здесь можно использовать свойство CategoryValues
// чтобы получить категории, фактически отображаемые в интерфейсе Excel
// в виде двумерного массива.
//Vector<Vector<ChartDataValue>> v1 = chart.GetNSeries().Get(0).GetCategoryValues();
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [ChartDataValue](../../chartdatavalue/)
* Class [Series](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
