---
title: Aspose::Cells::Drawing::Area::SetInvertIfNegative method
linktitle: SetInvertIfNegative
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Area::SetInvertIfNegative method. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged in C++.'
type: docs
weight: 1300
url: /tr/cpp/aspose.cells.drawing/area/setinvertifnegative/
---
## Area::SetInvertIfNegative method


If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```cpp
void Aspose::Cells::Drawing::Area::SetInvertIfNegative(bool value)
```


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
worksheet.GetCells().Get(u"A2").PutValue(-100);
//\"A3\" hücresine örnek bir değer ekleniyor
worksheet.GetCells().Get(u"A3").PutValue(150);
//Çalışma sayfasına bir grafik ekleniyor
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//Yeni eklenen grafiğin örneğine erişiliyor
Chart chart = worksheet.GetCharts().Get(chartIndex);
//\"A1\" hücresinden \"A3\" hücresine kadar olan aralıkta grafiğe NSeries (grafik veri kaynağı) ekleniyor
chart.GetNSeries().Add(u"A1:A3", true);
bool isNegative = chart.GetNSeries().Get(0).GetArea().GetInvertIfNegative();
chart.GetNSeries().Get(0).GetArea().SetInvertIfNegative(true);
//1. NSeries alanının ön plan rengini ayarlama
chart.GetNSeries().Get(0).GetArea().SetForegroundColor(Color{ 0xff, 0xff, 0, 0 });
//1. NSeries alanının arka plan rengini ayarlama.
//İkinci grafik noktasının gösterilen alan rengi arka plan rengi olacaktır.
chart.GetNSeries().Get(0).GetArea().SetBackgroundColor(Color{ 0xff, 0xff, 0xff, 0 });
//Excel dosyasını kaydetme
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Class [Area](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
