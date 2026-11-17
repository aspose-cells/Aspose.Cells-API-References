---
title: "Класс SeriesCollection"
linktitle: "SeriesCollection"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс SeriesCollection. Инкапсулирует объект, представляющий seriescollection в Go."
type: docs
weight: 200
url: /ru/go-cpp/seriescollection/
---

## SeriesCollection class

Инкапсулирует коллекцию объектов <see cref=\"Series\"/>.

```go

type SeriesCollection struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [Get](./get/) | Получает элемент Series по указанному индексу. |
| [GetSeriesByOrder](./getseriesbyorder/) | Получает элемент Series по порядку. |
| [RemoveAt](./removeat/) | Удалить серию по указанному индексу. |
| [GetCategoryData](./getcategorydata/) | Получает или задает диапазон значений оси категорий. Это может быть диапазон ячеек (например, "d1:e10") или последовательность значений (например, "{2,6,8,10}"). |
| [SetCategoryData](./setcategorydata/) | Получает или задает диапазон значений оси категорий. Это может быть диапазон ячеек (например, "d1:e10") или последовательность значений (например, "{2,6,8,10}"). |
| [GetSecondCategoryData](./getsecondcategorydata/) | Получает или задает диапазон значений второй оси категорий. Это может быть диапазон ячеек (например, "d1:e10"), или последовательность значений (например, "{2,6,8,10}"). Действует только когда некоторые серии построены на второй оси. |
| [SetSecondCategoryData](./setsecondcategorydata/) | Получает или задает диапазон значений второй оси категорий. Это может быть диапазон ячеек (например, "d1:e10"), или последовательность значений (например, "{2,6,8,10}"). Действует только когда некоторые серии построены на второй оси. |
| [SwapSeries](./swapseries/) | Непосредственно изменяет порядок двух серий. |
| [SetSeriesNames](./setseriesnames/) | Устанавливает имена всех серий на диаграмме. |
| [AddR1C1](./addr1c1/) | Добавляет коллекцию Series к диаграмме. |
| [Add_String_Bool](./add_string_bool/) | Добавляет коллекцию Series к диаграмме. |
| [Add_String_Bool_Bool](./add_string_bool_bool/) | Добавляет коллекцию Series к диаграмме. |
| [IsColorVaried](./iscolorvaried/) | Указывает, изменяется ли цвет точек. |
| [SetIsColorVaried](./setiscolorvaried/) | Указывает, изменяется ли цвет точек. |
| [Clear](./clear/) | Очищает коллекцию |
| [ChangeColors](./changecolors/) | Устанавливает монохромную палитру для серий диаграммы. |
| [GetCount](./getcount/) | Получает количество элементов, содержащихся в экземпляре. |
