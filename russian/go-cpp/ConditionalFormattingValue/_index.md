---
title: "Класс ConditionalFormattingValue"
linktitle: "ConditionalFormattingValue"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс ConditionalFormattingValue. Инкапсулирует объект, представляющий conditionalformattingvalue в Go."
type: docs
weight: 200
url: /ru/go-cpp/conditionalformattingvalue/
---

## ConditionalFormattingValue class

Описывает значения точек интерполяции в градиентной шкале, dataBar или iconSet.

```go

type ConditionalFormattingValue struct  {
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
| [GetValue](./getvalue/) | Получить или установить значение этого объекта условного форматирования. Его следует использовать вместе с Type. |
| [SetValue](./setvalue/) | Получить или установить значение этого объекта условного форматирования. Его следует использовать вместе с Type. |
| [GetType](./gettype/) | Получить или установить тип этого объекта условного форматирования. Установка типа в FormatConditionValueType.Min или FormatConditionValueType.Max автоматически установит \"Value\" в null. |
| [SetType](./settype/) | Получить или установить тип этого объекта условного форматирования. Установка типа в FormatConditionValueType.Min или FormatConditionValueType.Max автоматически установит \"Value\" в null. |
| [IsGTE](./isgte/) | Получить или установить флаг \"Больше или равно\". Используется только для наборов значков, определяет, использует ли это пороговое значение оператор \"больше или равно\". Значение 'false' указывает, что используется \"больше\", а не \"больше или равно\". Значение по умолчанию — true. |
| [SetIsGTE](./setisgte/) | Получить или установить флаг \"Больше или равно\". Используется только для наборов значков, определяет, использует ли это пороговое значение оператор \"больше или равно\". Значение 'false' указывает, что используется \"больше\", а не \"больше или равно\". Значение по умолчанию — true. |
