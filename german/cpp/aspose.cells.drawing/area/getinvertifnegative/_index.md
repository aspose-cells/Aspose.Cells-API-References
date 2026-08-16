---
title: Aspose::Cells::Drawing::Area::GetInvertIfNegative method
linktitle: GetInvertIfNegative
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Area::GetInvertIfNegative method. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged in C++.'
type: docs
weight: 1200
url: /de/cpp/aspose.cells.drawing/area/getinvertifnegative/
---
## Area::GetInvertIfNegative method


If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```cpp
bool Aspose::Cells::Drawing::Area::GetInvertIfNegative()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Instanziieren eines Workbook-Objekts
Workbook workbook;
//Adding a new worksheet to the Workbook object
int sheetIndex = workbook.GetWorksheets().Add();
//Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergeben seines Blattindexes
Worksheet worksheet = workbook.GetWorksheets().Get(sheetIndex);
//Beispielwert zur Zelle "A1" hinzufügen
worksheet.GetCells().Get(u"A1").PutValue(50);
//Beispielwert zur Zelle "A2" hinzufügen
worksheet.GetCells().Get(u"A2").PutValue(-100);
//Beispielwert zur Zelle "A3" hinzufügen
worksheet.GetCells().Get(u"A3").PutValue(150);
//Diagramm zum Arbeitsblatt hinzufügen
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//Zugriff auf die Instanz des neu hinzugefügten Diagramms
Chart chart = worksheet.GetCharts().Get(chartIndex);
//Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm vom Feld "A1" bis "A3"
chart.GetNSeries().Add(u"A1:A3", true);
bool isNegative = chart.GetNSeries().Get(0).GetArea().GetInvertIfNegative();
Aspose::Cells::Cleanup();
```

## See Also

* Class [Area](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
