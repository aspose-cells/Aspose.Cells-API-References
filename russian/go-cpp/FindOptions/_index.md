---
title: "FindOptions Class"
linktitle: "FindOptions"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "FindOptions class. Инкапсулирует объект, представляющий findoptions в Go."
type: docs
weight: 200
url: /ru/go-cpp/findoptions/
---

## FindOptions class

Представляет параметры поиска.

```go

type FindOptions struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewFindOptions](./newfindoptions/) | Конструктор по умолчанию. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetCaseSensitive](./getcasesensitive/) | Указывает, является ли искомая строка чувствительной к регистру. |
| [SetCaseSensitive](./setcasesensitive/) | Указывает, является ли искомая строка чувствительной к регистру. |
| [GetLookAtType](./getlookattype/) | Смотреть тип. |
| [SetLookAtType](./setlookattype/) | Смотреть тип. |
| [GetRange](./getrange/) | Получает и задает искомый диапазон. |
| [SetRange](./setrange/) | Задает искомый диапазон. |
| [IsRangeSet](./israngeset/) | Указывает, установлен ли искомый диапазон. |
| [GetSearchBackward](./getsearchbackward/) | Искать в обратном порядке для ячеек. |
| [SetSearchBackward](./setsearchbackward/) | Искать в обратном порядке для ячеек. |
| [GetSearchOrderByRows](./getsearchorderbyrows/) | Указывает, осуществляется ли поиск по строкам или столбцам. |
| [SetSearchOrderByRows](./setsearchorderbyrows/) | Указывает, осуществляется ли поиск по строкам или столбцам. |
| [GetLookInType](./getlookintype/) | Смотреть в типе. |
| [SetLookInType](./setlookintype/) | Смотреть в типе. |
| [GetRegexKey](./getregexkey/) | Указывает, является ли искомый ключ регулярным выражением. Если true, искомый ключ будет восприниматься как регулярное выражение и разбиратьcя. В противном случае ключ будет разбиратьcя согласно правилам MS Excel. |
| [SetRegexKey](./setregexkey/) | Указывает, является ли искомый ключ регулярным выражением. Если true, искомый ключ будет восприниматься как регулярное выражение и разбиратьcя. В противном случае ключ будет разбиратьcя согласно правилам MS Excel. |
| [GetValueTypeSensitive](./getvaluetypesensitive/) | Указывает, должен ли тип значения искомой ячейки совпадать с искомым ключом. |
| [SetValueTypeSensitive](./setvaluetypesensitive/) | Указывает, должен ли тип значения искомой ячейки совпадать с искомым ключом. |
| [GetStyle](./getstyle/) | Формат для поиска. |
| [SetStyle](./setstyle/) | Формат для поиска. |
| [GetConvertNumericData](./getconvertnumericdata/) | Получает или задает значение, указывающее, следует ли преобразовывать значение искомой строки в числовые данные. |
| [SetConvertNumericData](./setconvertnumericdata/) | Получает или задает значение, указывающее, следует ли преобразовывать значение искомой строки в числовые данные. |
