---
title: "Класс SettableGlobalizationSettings"
linktitle: "SettableGlobalizationSettings"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс SettableGlobalizationSettings. Инкапсулирует объект, представляющий settableglobalizationsettings в Go."
type: docs
weight: 200
url: /ru/go-cpp/settableglobalizationsettings/
---

## SettableGlobalizationSettings class

Реализация GlobalizationSettings, позволяющая пользователю задавать/изменять предопределённые тексты.

```go

type SettableGlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewSettableGlobalizationSettings](./newsettableglobalizationsettings/) | Конструктор по умолчанию. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetTotalName](./gettotalname/) | Получает полное имя конкретной функции. |
| [SetTotalName](./settotalname/) | Устанавливает полное имя конкретной функции. |
| [GetGrandTotalName](./getgrandtotalname/) | Получает название общего итога функции. |
| [SetGrandTotalName](./setgrandtotalname/) | Устанавливает название общего итога конкретной функции. |
| [GetTableRowTypeOfHeaders](./gettablerowtypeofheaders/) | Получает имя типа строк таблицы, состоящих из заголовка таблицы. По умолчанию "Headers", поэтому в формуле "#Headers" представляет заголовок таблицы. |
| [SetTableRowTypeOfHeaders](./settablerowtypeofheaders/) | Устанавливает имя типа строк таблицы, состоящих из заголовка таблицы. |
| [GetTableRowTypeOfData](./gettablerowtypeofdata/) | Получает имя типа строк таблицы, состоящих из области данных ссылочной таблицы. По умолчанию "Data", поэтому в формуле "#Data" представляет область данных таблицы. |
| [SetTableRowTypeOfData](./settablerowtypeofdata/) | Устанавливает имя типа строк таблицы, состоящих из области данных ссылочной таблицы. |
| [GetTableRowTypeOfAll](./gettablerowtypeofall/) | Получает имя типа строк таблицы, состоящих из всех строк в ссылочной таблице. |
| [SetTableRowTypeOfAll](./settablerowtypeofall/) | Устанавливает имя типа строк таблицы, состоящих из всех строк в ссылочной таблице. |
| [GetTableRowTypeOfTotals](./gettablerowtypeoftotals/) | Получает имя типа строк таблицы, состоящих из строки итога в ссылочной таблице. |
| [SetTableRowTypeOfTotals](./settablerowtypeoftotals/) | Устанавливает имя типа строк таблицы, состоящих из строки итога в ссылочной таблице. |
| [GetTableRowTypeOfCurrent](./gettablerowtypeofcurrent/) | Получает имя типа строк таблицы, состоящих из текущей строки в ссылочной таблице. |
| [SetTableRowTypeOfCurrent](./settablerowtypeofcurrent/) | Устанавливает имя типа строк таблицы, состоящих из текущей строки в ссылочной таблице. |
| [GetErrorValueString](./geterrorvaluestring/) | Получает строковое значение отображения для ошибочного значения ячейки. |
| [GetBooleanValueString](./getbooleanvaluestring/) | Получает строковое значение отображения для логического значения ячейки. |
| [SetBooleanValueString](./setbooleanvaluestring/) | Устанавливает строковое значение отображения для логического значения ячейки. |
| [GetLocalFunctionName](./getlocalfunctionname/) | Получает зависящее от локали имя функции в соответствии с заданным стандартным именем функции. |
| [SetLocalFunctionName](./setlocalfunctionname/) | Устанавливает зависящее от локали имя функции, соответствующее заданному стандартному имени функции. |
| [GetStandardFunctionName](./getstandardfunctionname/) | Получает стандартное имя функции в соответствии с заданным зависящим от локали именем функции. |
| [SetStandardFunctionName](./setstandardfunctionname/) | Устанавливает зависящее от локали имя функции в соответствии с заданным стандартным именем функции. |
| [GetLocalBuiltInName](./getlocalbuiltinname/) | Получает зависящий от локали текст для встроенного имени в соответствии с заданным стандартным текстом. |
| [SetLocalBuiltInName](./setlocalbuiltinname/) | Устанавливает зависящий от локали текст для встроенного имени с заданным стандартным текстом имени. |
| [GetStandardBuiltInName](./getstandardbuiltinname/) | Получает стандартный текст встроенного имени в соответствии с заданным зависящим от локали текстом. |
| [SetStandardBuiltInName](./setstandardbuiltinname/) | Устанавливает зависящее от локали имя функции в соответствии с заданным стандартным именем функции. |
| [GetListSeparator](./getlistseparator/) | Получает разделитель для списка, параметров функции и т.д. |
| [SetListSeparator](./setlistseparator/) | Устанавливает разделитель для списка, параметров функции и т.д. |
| [GetRowSeparatorOfFormulaArray](./getrowseparatorofformulaarray/) | Получает разделитель для строк в массивных данных в формуле. |
| [SetRowSeparatorOfFormulaArray](./setrowseparatorofformulaarray/) | Устанавливает разделитель для строк в массивных данных в формуле. |
| [GetColumnSeparatorOfFormulaArray](./getcolumnseparatorofformulaarray/) | Получает разделитель для элементов в строковых данных массива в формуле. |
| [SetColumnSeparatorOfFormulaArray](./setcolumnseparatorofformulaarray/) | Устанавливает разделитель для элементов в строковых данных массива в формуле. |
| [GetStandardHeaderFooterFontStyleName](./getstandardheaderfooterfontstylename/) | Получает стандартное английское название стиля шрифта (Regular, Bold, Italic) для Header/Footer в соответствии с указанным локализованным названием стиля шрифта. |
| [SetStandardHeaderFooterFontStyleName](./setstandardheaderfooterfontstylename/) | Устанавливает зависящее от локали имя функции в соответствии с заданным стандартным именем функции. |
| [GetCommentTitleName](./getcommenttitlename/) | Получает название заголовка комментария, зависящее от локали, в соответствии с типом заголовка комментария. |
| [SetCommentTitleName](./setcommenttitlename/) | Получает название заголовка комментария, зависящее от локали, в соответствии с типом заголовка комментария. |
