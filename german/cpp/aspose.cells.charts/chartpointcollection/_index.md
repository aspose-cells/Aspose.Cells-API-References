---
title: Aspose::Cells::Charts::ChartPointCollection class
linktitle: ChartPointCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::ChartPointCollection class. Represents a collection that contains all the points in one series in C++.'
type: docs
weight: 1100
url: /de/cpp/aspose.cells.charts/chartpointcollection/
---
## ChartPointCollection class


Represents a collection that contains all the points in one series.

```cpp
class ChartPointCollection
```

## Methods

| Method | Description |
| --- | --- |
| [ChartPointCollection(ChartPointCollection_Impl* impl)](./chartpointcollection/) | Constructs from an implementation object. |
| [ChartPointCollection(const ChartPointCollection\& src)](./chartpointcollection/) | Copy constructor. |
| [Clear()](./clear/) | Remove all setting of the chart points. |
| [Get(int32_t index)](./get/) | Gets the [ChartPoint](../chartpoint/) element at the specified index in the series. |
| [GetCount()](./getcount/) | Gets the count of the chart point. |
| [GetEnumerator()](./getenumerator/) | Returns an enumerator for the entire [ChartPointCollection](./). |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ChartPointCollection\& src)](./operator_asm/) | operator= |
| [RemoveAt(int32_t index)](./removeat/) | Removes point at the index of the series.. |
| [~ChartPointCollection()](./~chartpointcollection/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Instanziieren eines Workbook-Objekts
Workbook workbook;

//Abrufen der Referenz des ersten Arbeitsblatts
Worksheet worksheet = workbook.GetWorksheets().Get(0);

//Beispielwert zur Zelle "A1" hinzufügen
worksheet.GetCells().Get(u"A1").PutValue(50);

//Beispielwert zur Zelle "A2" hinzufügen
worksheet.GetCells().Get(u"A2").PutValue(100);

//Beispielwert zur Zelle "A3" hinzufügen
worksheet.GetCells().Get(u"A3").PutValue(150);

//Beispielwert zur Zelle "B1" hinzufügen
worksheet.GetCells().Get(u"B1").PutValue(60);

//Beispielwert zur Zelle "B2" hinzufügen
worksheet.GetCells().Get(u"B2").PutValue(32);

//Beispielwert zur Zelle "B3" hinzufügen
worksheet.GetCells().Get(u"B3").PutValue(50);

//Diagramm zum Arbeitsblatt hinzufügen
int chartIndex = worksheet.GetCharts().Add(ChartType::PieExploded, 5, 0, 25, 10);

//Zugriff auf die Instanz des neu hinzugefügten Diagramms
Chart chart = worksheet.GetCharts().Get(chartIndex);

//Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm im Bereich von Zelle "A1" bis "B3"
chart.GetNSeries().Add(u"A1:B3", true);

//Datenbeschriftungen anzeigen
chart.GetNSeries().Get(0).GetDataLabels().SetShowValue(true);

ChartPointCollection points = chart.GetNSeries().Get(0).GetPoints();

for (int i = 0; i < points.GetCount(); i++)
{
    //Datenpunkt abrufen
    ChartPoint point = points.Get(i);
    //Pir-Explosion festlegen
    point.SetExplosion(15);
    //Randfarbe festlegen
    point.GetBorder().SetColor(Color{ 0xff, 0xff, 0, 0 });
}

//Speichern der Excel-Datei
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
