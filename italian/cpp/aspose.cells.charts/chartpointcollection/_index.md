---
title: Aspose::Cells::Charts::ChartPointCollection class
linktitle: ChartPointCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::ChartPointCollection class. Represents a collection that contains all the points in one series in C++.'
type: docs
weight: 1100
url: /it/cpp/aspose.cells.charts/chartpointcollection/
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
//Istanziare un oggetto Workbook
Workbook workbook;

//Obtaining the reference of the first worksheet
Worksheet worksheet = workbook.GetWorksheets().Get(0);

//Aggiunta di un valore di esempio alla cella "A1"
worksheet.GetCells().Get(u"A1").PutValue(50);

//Aggiunta di un valore di esempio alla cella "A2"
worksheet.GetCells().Get(u"A2").PutValue(100);

//Aggiunta di un valore di esempio alla cella "A3"
worksheet.GetCells().Get(u"A3").PutValue(150);

//Aggiunta di un valore di esempio alla cella "B1"
worksheet.GetCells().Get(u"B1").PutValue(60);

//Aggiunta di un valore di esempio alla cella "B2"
worksheet.GetCells().Get(u"B2").PutValue(32);

//Aggiunta di un valore di esempio alla cella "B3"
worksheet.GetCells().Get(u"B3").PutValue(50);

//Aggiunta di un grafico al foglio di lavoro
int chartIndex = worksheet.GetCharts().Add(ChartType::PieExploded, 5, 0, 25, 10);

//Accesso all'istanza del grafico appena aggiunto
Chart chart = worksheet.GetCharts().Get(chartIndex);

//Aggiungere NSeries (origine dati del grafico) al grafico dall'intervallo di celle "A1" a "B3"
chart.GetNSeries().Add(u"A1:B3", true);

//Mostra etichette dati
chart.GetNSeries().Get(0).GetDataLabels().SetShowValue(true);

ChartPointCollection points = chart.GetNSeries().Get(0).GetPoints();

for (int i = 0; i < points.GetCount(); i++)
{
    //Ottieni punto dati
    ChartPoint point = points.Get(i);
    //Imposta esplosione Pir
    point.SetExplosion(15);
    //Imposta colore bordo
    point.GetBorder().SetColor(Color{ 0xff, 0xff, 0, 0 });
}

//Saving the Excel file
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
