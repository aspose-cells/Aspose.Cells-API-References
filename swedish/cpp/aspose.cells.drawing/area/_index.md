---
title: Aspose::Cells::Drawing::Area class
linktitle: Area
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Area class. Encapsulates the object that represents an area format in C++.'
type: docs
weight: 200
url: /sv/cpp/aspose.cells.drawing/area/
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
//Instansiering av ett Workbook-objekt
Workbook workbook;
//Lägger till ett nytt kalkylblad till Workbook-objektet
int sheetIndex = workbook.GetWorksheets().Add();
//Hämtar referensen till det nyligen tillagda kalkylbladet genom att ange dess bladindex.
Worksheet worksheet = workbook.GetWorksheets().Get(sheetIndex);
//Lägger till ett exempelvärde i cellen "A1"
worksheet.GetCells().Get(u"A1").PutValue(50);
//Lägger till ett exempelvärde i cellen "A2"
worksheet.GetCells().Get(u"A2").PutValue(100);
//Lägger till ett exempelvärde i cellen "A3"
worksheet.GetCells().Get(u"A3").PutValue(150);
//Lägger till ett exempelvärde i cellen "B1"
worksheet.GetCells().Get(u"B1").PutValue(60);
//Lägger till ett exempelvärde i cellen "B2"
worksheet.GetCells().Get(u"B2").PutValue(32);
//Lägger till ett exempelvärde i cellen "B3"
worksheet.GetCells().Get(u"B3").PutValue(50);
//Lägga till ett diagram i kalkylbladet
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//Åtkomst till instansen av det nyss tillagda diagrammet
Chart chart = worksheet.GetCharts().Get(chartIndex);
//Lägga till NSeries (diagramdatakälla) till diagrammet från cellen "A1" till "B3"
chart.GetNSeries().Add(u"A1:B3", true);
//Ställer in förgrundsfärgen för diagramområdet
chart.GetPlotArea().GetArea().SetForegroundColor(Color{ 0xff, 0, 0, 0xff });//Blue
//Ställer in förgrundsfärgen för diagramområdet
chart.GetChartArea().GetArea().SetForegroundColor(Color{ 0xff, 0xff, 0xff, 0 });//Yellow
//Ställer in förgrundsfärgen för den 1:a NSeries-området
chart.GetNSeries().Get(0).GetArea().SetForegroundColor(Color{ 0xff, 0xff, 0, 0 });//Red
//Ställer in förgrundsfärgen för området för den 1:a NSeries-punkten
chart.GetNSeries().Get(0).GetPoints().Get(0).GetArea().SetForegroundColor(Color{ 0xff, 0, 0xff, 0xff });//Cyan
//Sparar Excel-filen
workbook.Save(u"book1.xls");
Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Drawing](../)
* Library [Aspose.Cells for C++](../../)
