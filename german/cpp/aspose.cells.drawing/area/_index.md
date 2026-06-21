---
title: Aspose::Cells::Drawing::Area class
linktitle: Area
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Area class. Encapsulates the object that represents an area format in C++.'
type: docs
weight: 200
url: /de/cpp/aspose.cells.drawing/area/
---
## Area class


Encapsulates the object that represents an area format.

```cpp
class Area
```

## Methods

| Method | Description |
| --- | --- |
| [Area(Area_Impl* impl)](./area/) | Constructs from an implementation object. |
| [Area(const Area\& src)](./area/) | Copy constructor. |
| [GetBackgroundColor()](./getbackgroundcolor/) | Gets or sets the background [Color](../../aspose.cells/color/) of the [Area](./). |
| [GetFillFormat()](./getfillformat/) | Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape. |
| [GetForegroundColor()](./getforegroundcolor/) | Gets or sets the foreground [Color](../../aspose.cells/color/). |
| [GetFormatting()](./getformatting/) | Represents the formatting of the area. |
| [GetInvertIfNegative()](./getinvertifnegative/) | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [GetTransparency()](./gettransparency/) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Area\& src)](./operator_asm/) | operator= |
| [SetBackgroundColor(const Aspose::Cells::Color\& value)](./setbackgroundcolor/) | Gets or sets the background [Color](../../aspose.cells/color/) of the [Area](./). |
| [SetForegroundColor(const Aspose::Cells::Color\& value)](./setforegroundcolor/) | Gets or sets the foreground [Color](../../aspose.cells/color/). |
| [SetFormatting(FormattingType value)](./setformatting/) | Represents the formatting of the area. |
| [SetInvertIfNegative(bool value)](./setinvertifnegative/) | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [SetTransparency(double value)](./settransparency/) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [~Area()](./~area/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

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
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//Zugriff auf die Instanz des neu hinzugefügten Diagramms
Chart chart = worksheet.GetCharts().Get(chartIndex);
//Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm im Bereich von Zelle "A1" bis "B3"
chart.GetNSeries().Add(u"A1:B3", true);
//Setting the foreground color of the plot area
chart.GetPlotArea().GetArea().SetForegroundColor(Color{ 0xff, 0, 0, 0xff });//Blue
//Festlegen der Vordergrundfarbe des Diagrammbereichs
chart.GetChartArea().GetArea().SetForegroundColor(Color{ 0xff, 0xff, 0xff, 0 });//Yellow
//Setting the foreground color of the 1st NSeries area
chart.GetNSeries().Get(0).GetArea().SetForegroundColor(Color{ 0xff, 0xff, 0, 0 });//Red
//Setting the foreground color of the area of the 1st NSeries point
chart.GetNSeries().Get(0).GetPoints().Get(0).GetArea().SetForegroundColor(Color{ 0xff, 0, 0xff, 0xff });//Cyan
//Speichern der Excel-Datei
workbook.Save(u"book1.xls");
Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Drawing](../)
* Library [Aspose.Cells for C++](../../)
