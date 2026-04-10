---
title: Aspose::Cells::Drawing::Area::GetInvertIfNegative method
linktitle: GetInvertIfNegative
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Area::GetInvertIfNegative method. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged in C++.'
type: docs
weight: 1200
url: /ru/cpp/aspose.cells.drawing/area/getinvertifnegative/
---
## Area::GetInvertIfNegative method


If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```cpp
bool Aspose::Cells::Drawing::Area::GetInvertIfNegative()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Создание экземпляра объекта Workbook
Workbook workbook;
//Добавление нового листа в объект Workbook
int sheetIndex = workbook.GetWorksheets().Add();
//Получение ссылки на только что добавленный лист путем передачи его индекса листа
Worksheet worksheet = workbook.GetWorksheets().Get(sheetIndex);
//Добавление примерного значения в ячейку "A1"
worksheet.GetCells().Get(u"A1").PutValue(50);
//Добавление примерного значения в ячейку "A2"
worksheet.GetCells().Get(u"A2").PutValue(-100);
//Добавление примерного значения в ячейку "A3"
worksheet.GetCells().Get(u"A3").PutValue(150);
//Добавление диаграммы в рабочий лист
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//Доступ к экземпляру недавно добавленной диаграммы
Chart chart = worksheet.GetCharts().Get(chartIndex);
//Добавление NSeries (источник данных диаграммы) к диаграмме в диапазоне от ячейки \"A1\" до \"A3\"
chart.GetNSeries().Add(u"A1:A3", true);
bool isNegative = chart.GetNSeries().Get(0).GetArea().GetInvertIfNegative();
Aspose::Cells::Cleanup();
```

## See Also

* Class [Area](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
