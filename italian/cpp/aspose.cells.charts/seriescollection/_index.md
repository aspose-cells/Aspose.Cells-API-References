---
title: Aspose::Cells::Charts::SeriesCollection class
linktitle: SeriesCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::SeriesCollection class. Encapsulates a collection of Series objects in C++.'
type: docs
weight: 2600
url: /it/cpp/aspose.cells.charts/seriescollection/
---
## SeriesCollection class


Encapsulates a collection of [Series](../series/) objects.

```cpp
class SeriesCollection
```

## Methods

| Method | Description |
| --- | --- |
| [Add(const U16String\& dataArea, bool isVertical)](./add/) | Adds the [Series](../series/) collection to a chart. |
| [Add(const char16_t* dataArea, bool isVertical)](./add/) | Adds the [Series](../series/) collection to a chart. |
| [Add(const U16String\& area, bool isVertical, bool checkLabels)](./add/) | Adds the [Series](../series/) collection to a chart. |
| [Add(const char16_t* area, bool isVertical, bool checkLabels)](./add/) | Adds the [Series](../series/) collection to a chart. |
| [AddR1C1(const U16String\& area, bool isVertical)](./addr1c1/) | Adds the [Series](../series/) collection to a chart. |
| [AddR1C1(const char16_t* area, bool isVertical)](./addr1c1/) | Adds the [Series](../series/) collection to a chart. |
| [ChangeColors(ChartColorPaletteType type)](./changecolors/) | Set Monochromatic Palette for chart series. |
| [ChangeSeriesOrder(int32_t sourceIndex, int32_t destIndex)](./changeseriesorder/) |  **(Deprecated)** Directly changes the orders of the two series. |
| [Clear()](./clear/) | Clears the collection. |
| [Get(int32_t index)](./get/) | Gets the [Series](../series/) element at the specified index. |
| [GetCategoryData()](./getcategorydata/) | Gets or sets the range of category [Axis](../axis/) values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). |
| [GetCount()](./getcount/) |  |
| [GetSecondCategoryData()](./getsecondcategorydata/) | Gets or sets the range of second category [Axis](../axis/) values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some series were plotted on the second axis. |
| [GetSeriesByOrder(int32_t order)](./getseriesbyorder/) | Gets the [Series](../series/) element by order. |
| [IsColorVaried()](./iscolorvaried/) | Represents if the color of points is varied. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SeriesCollection\& src)](./operator_asm/) | operator= |
| [RemoveAt(int32_t index)](./removeat/) | Remove at a series at the specific index. |
| [SeriesCollection(SeriesCollection_Impl* impl)](./seriescollection/) | Constructs from an implementation object. |
| [SeriesCollection(const SeriesCollection\& src)](./seriescollection/) | Copy constructor. |
| [SetCategoryData(const U16String\& value)](./setcategorydata/) | Gets or sets the range of category [Axis](../axis/) values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). |
| [SetCategoryData(const char16_t* value)](./setcategorydata/) | Gets or sets the range of category [Axis](../axis/) values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). |
| [SetIsColorVaried(bool value)](./setiscolorvaried/) | Represents if the color of points is varied. |
| [SetSecondCategoryData(const U16String\& value)](./setsecondcategorydata/) | Gets or sets the range of second category [Axis](../axis/) values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some series were plotted on the second axis. |
| [SetSecondCategoryData(const char16_t* value)](./setsecondcategorydata/) | Gets or sets the range of second category [Axis](../axis/) values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some series were plotted on the second axis. |
| [SetSeriesNames(int32_t startIndex, const U16String\& area, bool isVertical)](./setseriesnames/) | Sets the name of all the serieses in the chart. |
| [SetSeriesNames(int32_t startIndex, const char16_t* area, bool isVertical)](./setseriesnames/) | Sets the name of all the serieses in the chart. |
| [SwapSeries(int32_t sourceIndex, int32_t destIndex)](./swapseries/) | Directly changes the orders of the two series. |
| [~SeriesCollection()](./~seriescollection/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Istanziare un oggetto Workbook
Workbook workbook;
//Aggiungere un nuovo foglio di lavoro all'oggetto Excel
int sheetIndex = workbook.GetWorksheets().Add();
//Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
Worksheet worksheet = workbook.GetWorksheets().Get(sheetIndex);
//Aggiunta di un valore di esempio alla cella "A1"
worksheet.GetCells().Get(u"A1").PutValue(50);
//Aggiunta di un valore di esempio alla cella "A2"
worksheet.GetCells().Get(u"A2").PutValue(100);
//Aggiunta di un valore di esempio alla cella "A3"
worksheet.GetCells().Get(u"A3").PutValue(150);
//Aggiunta di un valore di esempio alla cella "A4"
worksheet.GetCells().Get(u"A4").PutValue(200);
//Aggiunta di un valore di esempio alla cella "B1"
worksheet.GetCells().Get(u"B1").PutValue(60);
//Aggiunta di un valore di esempio alla cella "B2"
worksheet.GetCells().Get(u"B2").PutValue(32);
//Aggiunta di un valore di esempio alla cella "B3"
worksheet.GetCells().Get(u"B3").PutValue(50);
//Aggiunta di un valore di esempio alla cella "B4"
worksheet.GetCells().Get(u"B4").PutValue(40);
//Aggiunta di un valore di esempio alla cella "C1" come dati di categoria
worksheet.GetCells().Get(u"C1").PutValue(u"Q1");
//Aggiunta di un valore di esempio alla cella "C2" come dati di categoria
worksheet.GetCells().Get(u"C2").PutValue(u"Q2");
//Aggiunta di un valore di esempio alla cella "C3" come dati di categoria
worksheet.GetCells().Get(u"C3").PutValue(u"Y1");
//Aggiunta di un valore di esempio alla cella "C4" come dati di categoria
worksheet.GetCells().Get(u"C4").PutValue(u"Y2");
//Aggiunta di un grafico al foglio di lavoro
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//Accesso all'istanza del grafico appena aggiunto
Chart chart = worksheet.GetCharts().Get(chartIndex);
//Aggiunta di NSeries (origine dati del grafico) al grafico che va dalla cella "A1" alla "B4"
chart.GetNSeries().Add(u"A1:B4", true);
//Impostazione dell'origine dati per i dati di categoria di NSeries
chart.GetNSeries().SetCategoryData(u"C1:C4");
//Saving the Excel file
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
