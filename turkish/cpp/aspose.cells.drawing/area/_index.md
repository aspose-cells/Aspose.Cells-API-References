---
title: Aspose::Cells::Drawing::Area class
linktitle: Area
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Area class. Encapsulates the object that represents an area format in C++.'
type: docs
weight: 200
url: /tr/cpp/aspose.cells.drawing/area/
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
//Bir Workbook nesnesi oluşturuluyor
Workbook workbook;
//Workbook nesnesine yeni bir çalışma sayfası ekleme
int sheetIndex = workbook.GetWorksheets().Add();
//Yeni eklenen çalışma sayfasının referansını, sayfa indeksini geçirerek elde etme
Worksheet worksheet = workbook.GetWorksheets().Get(sheetIndex);
//\"A1\" hücresine örnek bir değer ekleniyor
worksheet.GetCells().Get(u"A1").PutValue(50);
//\"A2\" hücresine örnek bir değer ekleniyor
worksheet.GetCells().Get(u"A2").PutValue(100);
//\"A3\" hücresine örnek bir değer ekleniyor
worksheet.GetCells().Get(u"A3").PutValue(150);
//\"B1\" hücresine örnek bir değer ekleniyor
worksheet.GetCells().Get(u"B1").PutValue(60);
//\"B2\" hücresine örnek bir değer ekleniyor
worksheet.GetCells().Get(u"B2").PutValue(32);
//\"B3\" hücresine örnek bir değer ekleniyor
worksheet.GetCells().Get(u"B3").PutValue(50);
//Çalışma sayfasına bir grafik ekleniyor
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//Yeni eklenen grafiğin örneğine erişiliyor
Chart chart = worksheet.GetCharts().Get(chartIndex);
//Grafiğe "A1" hücresinden "B3" hücresine kadar NSeries (grafik veri kaynağı) ekleme
chart.GetNSeries().Add(u"A1:B3", true);
//Grafik alanının ön plan rengini ayarlama
chart.GetPlotArea().GetArea().SetForegroundColor(Color{ 0xff, 0, 0, 0xff });//Blue
//Grafik alanının ön plan rengini ayarlama
chart.GetChartArea().GetArea().SetForegroundColor(Color{ 0xff, 0xff, 0xff, 0 });//Yellow
//1. NSeries alanının ön plan rengini ayarlama
chart.GetNSeries().Get(0).GetArea().SetForegroundColor(Color{ 0xff, 0xff, 0, 0 });//Red
//1. NSeries noktasının alanının ön plan rengini ayarlama
chart.GetNSeries().Get(0).GetPoints().Get(0).GetArea().SetForegroundColor(Color{ 0xff, 0, 0xff, 0xff });//Cyan
//Excel dosyasını kaydetme
workbook.Save(u"book1.xls");
Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Drawing](../)
* Library [Aspose.Cells for C++](../../)
