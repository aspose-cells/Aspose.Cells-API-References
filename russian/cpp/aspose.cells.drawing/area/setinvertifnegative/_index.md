---
title: Aspose::Cells::Drawing::Area::SetInvertIfNegative method
linktitle: SetInvertIfNegative
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Area::SetInvertIfNegative method. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged in C++.'
type: docs
weight: 1300
url: /ru/cpp/aspose.cells.drawing/area/setinvertifnegative/
---
## Area::SetInvertIfNegative method


If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```cpp
void Aspose::Cells::Drawing::Area::SetInvertIfNegative(bool value)
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
chart.GetNSeries().Get(0).GetArea().SetInvertIfNegative(true);
//Установка цвета переднего плана области 1‑го NSeries
chart.GetNSeries().Get(0).GetArea().SetForegroundColor(Color{ 0xff, 0xff, 0, 0 });
//Установка фонового цвета первой области NSeries.
//Отображаемый цвет области второй точки диаграммы будет фоновым цветом.
chart.GetNSeries().Get(0).GetArea().SetBackgroundColor(Color{ 0xff, 0xff, 0xff, 0 });
//Сохранение файла Excel
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Class [Area](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
