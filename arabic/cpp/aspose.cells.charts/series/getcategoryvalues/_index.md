---
title: Aspose::Cells::Charts::Series::GetCategoryValues method
linktitle: GetCategoryValues
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::Series::GetCategoryValues method. Gets the actual category values that are used to plot every point of this series in the chart in C++.'
type: docs
weight: 2100
url: /ar/cpp/aspose.cells.charts/series/getcategoryvalues/
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
// قد تكون XValues مثل "[External.xlsx]Sheet1!$B$2:$C$6" وهو معقد
// لتمكين المستخدم من الحصول على القيم الفعلية (قد تكون القيم مرتبطة بكتاب عمل آخر،
// أو مخزنة مؤقتاً في كتاب العمل الحالي). هنا يمكنك استخدام الخاصية CategoryValues
// للحصول على قيم الفئات المعروضة فعلياً في واجهة Excel
// على شكل مصفوفة ثنائية الأبعاد.
//Vector<Vector<ChartDataValue>> v1 = chart.GetNSeries().Get(0).GetCategoryValues();
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [ChartDataValue](../../chartdatavalue/)
* Class [Series](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
