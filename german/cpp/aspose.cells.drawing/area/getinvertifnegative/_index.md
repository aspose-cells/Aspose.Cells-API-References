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
//Hinzufügen eines neuen Arbeitsblatts zum Workbook-Objekt
int sheetIndex = workbook.GetWorksheets().Add();
//Abrufen der Referenz des neu hinzugefügten Arbeitsblatts, indem dessen Blattindex übergeben wird
Worksheet worksheet = workbook.GetWorksheets().Get(sheetIndex);
//Füge einen Beispielwert zur Zelle "A1" hinzu
worksheet.GetCells().Get(u"A1").PutValue(50);
//Füge einen Beispielwert zur Zelle "A2" hinzu
worksheet.GetCells().Get(u"A2").PutValue(-100);
//Füge einen Beispielwert zur Zelle "A3" hinzu
worksheet.GetCells().Get(u"A3").PutValue(150);
//Hinzufügen eines Diagramms zum Arbeitsblatt
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//Zugriff auf die Instanz des neu hinzugefügten Diagramms
Chart chart = worksheet.GetCharts().Get(chartIndex);
//Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm im Bereich von Zelle "A1" bis "A3"
chart.GetNSeries().Add(u"A1:A3", true);
bool isNegative = chart.GetNSeries().Get(0).GetArea().GetInvertIfNegative();
chart.GetNSeries().Get(0).GetArea().SetInvertIfNegative(true);
//Festlegen der Vordergrundfarbe des 1. NSeries-Bereichs
chart.GetNSeries().Get(0).GetArea().SetForegroundColor(Color{ 0xff, 0xff, 0, 0 });
//Festlegen der Hintergrundfarbe des ersten NSeries‑Bereichs.
//Die angezeigte Flächenfarbe des zweiten Diagrammpunkts wird die Hintergrundfarbe sein.
chart.GetNSeries().Get(0).GetArea().SetBackgroundColor(Color{ 0xff, 0xff, 0xff, 0 });
//Speichern der Excel-Datei
workbook.Save(u"book1.xls");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Area](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
