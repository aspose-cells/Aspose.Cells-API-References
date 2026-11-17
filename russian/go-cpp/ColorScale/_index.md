---
title: "Класс ColorScale"
linktitle: "ColorScale"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс ColorScale. Инкапсулирует объект, представляющий colorscale в Go."
type: docs
weight: 200
url: /ru/go-cpp/colorscale/
---

## ColorScale class

Опишите правило условного форматирования ColorScale.Это правило условного форматирования создает градиентную цветовую шкалу в ячейках.

```go

type ColorScale struct  {
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
| [GetIs3ColorScale](./getis3colorscale/) | Указывает, является ли условное форматирование трехцветной шкалой. |
| [SetIs3ColorScale](./setis3colorscale/) | Указывает, является ли условное форматирование трехцветной шкалой. |
| [GetMinCfvo](./getmincfvo/) | Получить или установить объект минимального значения этого ColorScale. Нельзя установить null или CFValueObject с типом FormatConditionValueType.Max. |
| [GetMidCfvo](./getmidcfvo/) | Получить или установить объект среднего значения этого ColorScale. Нельзя установить CFValueObject с типом FormatConditionValueType.Max или FormatConditionValueType.Min. |
| [GetMaxCfvo](./getmaxcfvo/) | Получить или установить объект максимального значения этого ColorScale. Нельзя установить null или CFValueObject с типом FormatConditionValueType.Min. |
| [GetMinColor](./getmincolor/) | Получить или установить градиентный цвет для минимального значения в диапазоне. |
| [SetMinColor](./setmincolor/) | Получить или установить градиентный цвет для минимального значения в диапазоне. |
| [GetMidColor](./getmidcolor/) | Получить или установить градиентный цвет для среднего значения в диапазоне. |
| [SetMidColor](./setmidcolor/) | Получить или установить градиентный цвет для среднего значения в диапазоне. |
| [GetMaxColor](./getmaxcolor/) | Получить или установить градиентный цвет для максимального значения в диапазоне. |
| [SetMaxColor](./setmaxcolor/) | Получить или установить градиентный цвет для максимального значения в диапазоне. |
