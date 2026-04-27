---
title: Aspose::Cells::Charts::SeriesCollection class
linktitle: SeriesCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::SeriesCollection class. Encapsulates a collection of Series objects in C++.'
type: docs
weight: 2600
url: /fr/cpp/aspose.cells.charts/seriescollection/
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
//Instanciation d'un objet Workbook
Workbook workbook;
//Ajout d'une nouvelle feuille de calcul à l'objet Excel
int sheetIndex = workbook.GetWorksheets().Add();
//Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son index de feuille
Worksheet worksheet = workbook.GetWorksheets().Get(sheetIndex);
//Ajouter une valeur d'exemple à la cellule \"A1\"
worksheet.GetCells().Get(u"A1").PutValue(50);
//Ajouter une valeur d'exemple à la cellule \"A2\"
worksheet.GetCells().Get(u"A2").PutValue(100);
//Ajouter une valeur d'exemple à la cellule \"A3\"
worksheet.GetCells().Get(u"A3").PutValue(150);
//Ajouter une valeur d'exemple à la cellule \"A4\"
worksheet.GetCells().Get(u"A4").PutValue(200);
//Ajouter une valeur d'exemple à la cellule \"B1\"
worksheet.GetCells().Get(u"B1").PutValue(60);
//Ajouter une valeur d'exemple à la cellule \"B2\"
worksheet.GetCells().Get(u"B2").PutValue(32);
//Ajouter une valeur d'exemple à la cellule \"B3\"
worksheet.GetCells().Get(u"B3").PutValue(50);
//Ajouter une valeur d'exemple à la cellule \"B4\"
worksheet.GetCells().Get(u"B4").PutValue(40);
//Ajouter une valeur d'exemple à la cellule \"C1\" en tant que donnée de catégorie
worksheet.GetCells().Get(u"C1").PutValue(u"Q1");
//Ajouter une valeur d'exemple à la cellule \"C2\" en tant que donnée de catégorie
worksheet.GetCells().Get(u"C2").PutValue(u"Q2");
//Ajouter une valeur d'exemple à la cellule \"C3\" en tant que donnée de catégorie
worksheet.GetCells().Get(u"C3").PutValue(u"Y1");
//Ajouter une valeur d'exemple à la cellule \"C4\" en tant que donnée de catégorie
worksheet.GetCells().Get(u"C4").PutValue(u"Y2");
//Ajouter un graphique à la feuille de calcul
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//Accéder à l'instance du graphique nouvellement ajouté
Chart chart = worksheet.GetCharts().Get(chartIndex);
//Ajouter NSeries (source de données du graphique) au graphique allant de la cellule \"A1\" à \"B4\"
chart.GetNSeries().Add(u"A1:B4", true);
//Définir la source de données pour les données de catégorie de NSeries
chart.GetNSeries().SetCategoryData(u"C1:C4");
//Enregistrement du fichier Excel
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
