---
title: Aspose::Cells::Charts::ChartPointCollection class
linktitle: ChartPointCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::ChartPointCollection class. Represents a collection that contains all the points in one series in C++.'
type: docs
weight: 1100
url: /ru/cpp/aspose.cells.charts/chartpointcollection/
---
## ChartPointCollection class


Represents a collection that contains all the points in one series.

```cpp
class ChartPointCollection
```

## Methods

| Method | Description |
| --- | --- |
| [ChartPointCollection(ChartPointCollection_Impl* impl)](./chartpointcollection/) | Constructs from an implementation object. |
| [ChartPointCollection(const ChartPointCollection\& src)](./chartpointcollection/) | Copy constructor. |
| [Clear()](./clear/) | Remove all setting of the chart points. |
| [Get(int32_t index)](./get/) | Gets the [ChartPoint](../chartpoint/) element at the specified index in the series. |
| [GetCount()](./getcount/) | Gets the count of the chart point. |
| [GetEnumerator()](./getenumerator/) | Returns an enumerator for the entire [ChartPointCollection](./). |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ChartPointCollection\& src)](./operator_asm/) | operator= |
| [RemoveAt(int32_t index)](./removeat/) | Removes point at the index of the series.. |
| [~ChartPointCollection()](./~chartpointcollection/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Создание экземпляра объекта Workbook
Workbook workbook;

//Получение ссылки на первый лист
Worksheet worksheet = workbook.GetWorksheets().Get(0);

//Добавление примерного значения в ячейку "A1"
worksheet.GetCells().Get(u"A1").PutValue(50);

//Добавление примерного значения в ячейку "A2"
worksheet.GetCells().Get(u"A2").PutValue(100);

//Добавление примерного значения в ячейку "A3"
worksheet.GetCells().Get(u"A3").PutValue(150);

//Добавление примерного значения в ячейку "B1"
worksheet.GetCells().Get(u"B1").PutValue(60);

//Добавление примерного значения в ячейку "B2"
worksheet.GetCells().Get(u"B2").PutValue(32);

//Добавление примерного значения в ячейку "B3"
worksheet.GetCells().Get(u"B3").PutValue(50);

//Добавление диаграммы в рабочий лист
int chartIndex = worksheet.GetCharts().Add(ChartType::PieExploded, 5, 0, 25, 10);

//Доступ к экземпляру недавно добавленной диаграммы
Chart chart = worksheet.GetCharts().Get(chartIndex);

//Добавление NSeries (источник данных диаграммы) к диаграмме в диапазоне от ячейки "A1" до "B3"
chart.GetNSeries().Add(u"A1:B3", true);

//Показать подписи данных
chart.GetNSeries().Get(0).GetDataLabels().SetShowValue(true);

ChartPointCollection points = chart.GetNSeries().Get(0).GetPoints();

for (int i = 0; i < points.GetCount(); i++)
{
    //Получить точку данных
    ChartPoint point = points.Get(i);
    //Установить Pir Explosion
    point.SetExplosion(15);
    //Установить цвет границы
    point.GetBorder().SetColor(Color{ 0xff, 0xff, 0, 0 });
}

//Сохранение файла Excel
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
