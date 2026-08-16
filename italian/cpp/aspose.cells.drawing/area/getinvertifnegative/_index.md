---
title: Aspose::Cells::Drawing::Area::GetInvertIfNegative method
linktitle: GetInvertIfNegative
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Area::GetInvertIfNegative method. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged in C++.'
type: docs
weight: 1200
url: /it/cpp/aspose.cells.drawing/area/getinvertifnegative/
---
## Area::GetInvertIfNegative method


If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```cpp
bool Aspose::Cells::Drawing::Area::GetInvertIfNegative()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Istanziare un oggetto Workbook
Workbook workbook;
//Adding a new worksheet to the Workbook object
int sheetIndex = workbook.GetWorksheets().Add();
//Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
Worksheet worksheet = workbook.GetWorksheets().Get(sheetIndex);
//Aggiunta di un valore di esempio alla cella "A1"
worksheet.GetCells().Get(u"A1").PutValue(50);
//Aggiunta di un valore di esempio alla cella "A2"
worksheet.GetCells().Get(u"A2").PutValue(-100);
//Aggiunta di un valore di esempio alla cella "A3"
worksheet.GetCells().Get(u"A3").PutValue(150);
//Aggiunta di un grafico al foglio di lavoro
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//Accesso all'istanza del grafico appena aggiunto
Chart chart = worksheet.GetCharts().Get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "A3"
chart.GetNSeries().Add(u"A1:A3", true);
bool isNegative = chart.GetNSeries().Get(0).GetArea().GetInvertIfNegative();
Aspose::Cells::Cleanup();
```

## See Also

* Class [Area](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
