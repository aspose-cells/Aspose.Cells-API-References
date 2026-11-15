---
title: Aspose::Cells::Drawing::Area::GetInvertIfNegative method
linktitle: GetInvertIfNegative
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Area::GetInvertIfNegative method. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged in C++.'
type: docs
weight: 1200
url: /sv/cpp/aspose.cells.drawing/area/getinvertifnegative/
---
## Area::GetInvertIfNegative method


If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```cpp
bool Aspose::Cells::Drawing::Area::GetInvertIfNegative()
```


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
worksheet.GetCells().Get(u"A2").PutValue(-100);
//Lägger till ett exempelvärde i cellen "A3"
worksheet.GetCells().Get(u"A3").PutValue(150);
//Lägga till ett diagram i kalkylbladet
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//Åtkomst till instansen av det nyss tillagda diagrammet
Chart chart = worksheet.GetCharts().Get(chartIndex);
//Lägger till NSeries (diagramdatakälla) till diagrammet som sträcker sig från cell "A1" till "A3"
chart.GetNSeries().Add(u"A1:A3", true);
bool isNegative = chart.GetNSeries().Get(0).GetArea().GetInvertIfNegative();
chart.GetNSeries().Get(0).GetArea().SetInvertIfNegative(true);
//Ställer in förgrundsfärgen för den 1:a NSeries-området
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
