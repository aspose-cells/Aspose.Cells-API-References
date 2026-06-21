---
title: Aspose::Cells::Charts::Series::GetPointValues method
linktitle: GetPointValues
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::Series::GetPointValues method. Gets the actual values that are used to plot every point of this series in the chart in C++.'
type: docs
weight: 2000
url: /de/cpp/aspose.cells.charts/series/getpointvalues/
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
// Werte können z. B. "[External.xlsx]Sheet1!$A$1:$A$6" sein, was kompliziert ist
// für den Benutzer, um die tatsächlichen Werte zu erhalten (die Werte können mit einer anderen Arbeitsmappe verknüpft sein,
// oder im aktuellen Arbeitsbuch zwischengespeichert sein). Hier können Sie die Eigenschaft PointValues verwenden
// um die in der Excel‑Oberfläche tatsächlich angezeigten Werte zu erhalten
// in Form eines Arrays.
//Vector<ChartDataValue> v1 = chart.GetNSeries().Get(0).GetPointValues();
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [ChartDataValue](../../chartdatavalue/)
* Class [Series](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
