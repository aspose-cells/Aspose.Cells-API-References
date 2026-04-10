---
title: Aspose::Cells::Charts::Series::GetCategoryValues method
linktitle: GetCategoryValues
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::Series::GetCategoryValues method. Gets the actual category values that are used to plot every point of this series in the chart in C++.'
type: docs
weight: 2100
url: /es/cpp/aspose.cells.charts/series/getcategoryvalues/
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
// XValues puede ser como "[External.xlsx]Sheet1!$B$2:$C$6" lo cual es complicado
// para que el usuario obtenga los valores reales (los valores pueden estar vinculados a otro libro,
// o almacenados en caché en el libro actual). Aquí puede usar la propiedad CategoryValues
// para obtener los valores de categoría que se muestran realmente en la interfaz de Excel
// en forma de una matriz bidimensional.
//Vector<Vector<ChartDataValue>> v1 = chart.GetNSeries().Get(0).GetCategoryValues();
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [ChartDataValue](../../chartdatavalue/)
* Class [Series](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
