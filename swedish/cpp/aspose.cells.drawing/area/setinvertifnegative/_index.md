---
title: Aspose::Cells::Drawing::Area::SetInvertIfNegative method
linktitle: SetInvertIfNegative
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Area::SetInvertIfNegative method. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged in C++.'
type: docs
weight: 1300
url: /sv/cpp/aspose.cells.drawing/area/setinvertifnegative/
---
## Area::SetInvertIfNegative method


If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```cpp
void Aspose::Cells::Drawing::Area::SetInvertIfNegative(bool value)
```


## Examples


```cpp
Aspose::Cells::Startup();
//Instansierar ett Workbook‑objekt
Workbook workbook;
//Lägger till ett nytt kalkylblad till Workbook-objektet
int sheetIndex = workbook.GetWorksheets().Add();
//Hämtar referensen till det nyligen tillagda kalkylbladet genom att ange dess bladindex
Worksheet worksheet = workbook.GetWorksheets().Get(sheetIndex);
//Adding a sample value to "A1" cell
worksheet.GetCells().Get(u"A1").PutValue(50);
//Adding a sample value to "A2" cell
worksheet.GetCells().Get(u"A2").PutValue(-100);
//Adding a sample value to "A3" cell
worksheet.GetCells().Get(u"A3").PutValue(150);
//Adding a chart to the worksheet
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
Chart chart = worksheet.GetCharts().Get(chartIndex);
//Lägger till NSeries (diagramdatakälla) till diagrammet som sträcker sig från cell "A1" till "A3"
chart.GetNSeries().Add(u"A1:A3", true);
chart.GetNSeries().Get(0).GetArea().SetInvertIfNegative(true);
//Ställer in förgrundsfärgen för det första NSeries-området
chart.GetNSeries().Get(0).GetArea().SetForegroundColor(Color{ 0xff, 0xff, 0, 0 });
//Ställer in bakgrundsfärgen för det första NSeries-området.
//Den visade områdesfärgen för den andra diagrampunkten blir bakgrundsfärgen.
chart.GetNSeries().Get(0).GetArea().SetBackgroundColor(Color{ 0xff, 0xff, 0xff, 0 });
//Sparar Excel-filen
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Class [Area](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
