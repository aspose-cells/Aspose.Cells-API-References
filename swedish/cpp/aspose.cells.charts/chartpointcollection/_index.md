---
title: Aspose::Cells::Charts::ChartPointCollection class
linktitle: ChartPointCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::ChartPointCollection class. Represents a collection that contains all the points in one series in C++.'
type: docs
weight: 1100
url: /sv/cpp/aspose.cells.charts/chartpointcollection/
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
//Instansierar ett Workbook‑objekt
Workbook workbook;

//Hämtar referensen till det första kalkylbladet
Worksheet worksheet = workbook.GetWorksheets().Get(0);

//Adding a sample value to "A1" cell
worksheet.GetCells().Get(u"A1").PutValue(50);

//Adding a sample value to "A2" cell
worksheet.GetCells().Get(u"A2").PutValue(100);

//Adding a sample value to "A3" cell
worksheet.GetCells().Get(u"A3").PutValue(150);

//Adding a sample value to "B1" cell
worksheet.GetCells().Get(u"B1").PutValue(60);

//Adding a sample value to "B2" cell
worksheet.GetCells().Get(u"B2").PutValue(32);

//Adding a sample value to "B3" cell
worksheet.GetCells().Get(u"B3").PutValue(50);

//Adding a chart to the worksheet
int chartIndex = worksheet.GetCharts().Add(ChartType::PieExploded, 5, 0, 25, 10);

//Accessing the instance of the newly added chart
Chart chart = worksheet.GetCharts().Get(chartIndex);

//Lägger till NSeries (diagramdatakälla) i diagrammet från cell "A1" till "B3"
chart.GetNSeries().Add(u"A1:B3", true);

//Visa datamärkningar
chart.GetNSeries().Get(0).GetDataLabels().SetShowValue(true);

ChartPointCollection points = chart.GetNSeries().Get(0).GetPoints();

for (int i = 0; i < points.GetCount(); i++)
{
    //Hämta datapunkt
    ChartPoint point = points.Get(i);
    //Ställ in Pir Explosion
    point.SetExplosion(15);
    //Ställ in kantfärg
    point.GetBorder().SetColor(Color{ 0xff, 0xff, 0, 0 });
}

//Sparar Excel-filen
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
