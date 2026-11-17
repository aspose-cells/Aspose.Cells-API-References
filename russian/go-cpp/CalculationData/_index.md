---
title: "Класс CalculationData"
linktitle: "CalculationData"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс CalculationData. Инкапсулирует объект, представляющий calculationdata в Go."
type: docs
weight: 200
url: /ru/go-cpp/calculationdata/
---

## CalculationData class

Представляет необходимые данные при вычислении функции, такие как имя функции, параметры и т.д.

```go

type CalculationData struct  {
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
| [GetCalculatedValue](./getcalculatedvalue/) | Получает или задает вычисленное значение для этой функции. |
| [SetCalculatedValue](./setcalculatedvalue/) | Получает или задает вычисленное значение для этой функции. |
| [GetWorkbook](./getworkbook/) | Получает объект Workbook, в котором находится функция. |
| [GetWorksheet](./getworksheet/) | Получает объект Worksheet, в котором находится функция. |
| [GetCellRow](./getcellrow/) | Получает индекс строки ячейки, в которой находится функция. |
| [GetCellColumn](./getcellcolumn/) | Получает индекс столбца ячейки, в которой находится функция. |
| [GetCell](./getcell/) | Получает объект Cell, в котором находится функция. |
| [GetFunctionName](./getfunctionname/) | Получает имя функции для вычисления. |
| [GetParamCount](./getparamcount/) | Получает количество параметров |
| [GetParamValue](./getparamvalue/) | Получает представленный объект значения параметра по заданному индексу. |
| [GetParamValueInArrayMode](./getparamvalueinarraymode/) | Получает значение(я) параметра по заданному индексу.Если параметр представляет собой некоторый вид выражения, требующего вычисления, то оно будет вычислено в режиме массива. |
| [GetParamText](./getparamtext/) | Получает буквальный текст параметра по заданному индексу. |
