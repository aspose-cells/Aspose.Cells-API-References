---
title: "Класс GlobalizationSettings"
linktitle: "GlobalizationSettings"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс GlobalizationSettings. Инкапсулирует объект, представляющий настройки глобализации в Go."
type: docs
weight: 200
url: /ru/go-cpp/globalizationsettings/
---

## GlobalizationSettings class

Представляет настройки глобализации.

```go

type GlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewGlobalizationSettings](./newglobalizationsettings/) | Конструктор по умолчанию. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetChartSettings](./getchartsettings/) | Получает настройки глобализации для диаграммы. |
| [SetChartSettings](./setchartsettings/) | Устанавливает настройки глобализации для диаграммы. |
| [GetPivotSettings](./getpivotsettings/) | Получает настройки глобализации для сводной таблицы. |
| [SetPivotSettings](./setpivotsettings/) | Устанавливает настройки глобализации для сводной таблицы. |
| [GetTotalName](./gettotalname/) | Получает общее имя функции. |
| [GetGrandTotalName](./getgrandtotalname/) | Получает название общего итога функции. |
| [GetDefaultSheetName](./getdefaultsheetname/) | Получает имя листа по умолчанию для автоматического добавления листа. По умолчанию "Sheet". |
| [GetTableRowTypeOfHeaders](./gettablerowtypeofheaders/) | Получает имя типа строк таблицы, состоящих из заголовка таблицы. По умолчанию "Headers", поэтому в формуле "#Headers" представляет заголовок таблицы. |
| [GetTableRowTypeOfData](./gettablerowtypeofdata/) | Получает имя типа строк таблицы, состоящих из области данных ссылочной таблицы. По умолчанию "Data", поэтому в формуле "#Data" представляет область данных таблицы. |
| [GetTableRowTypeOfAll](./gettablerowtypeofall/) | Получает типовое имя строк таблицы, которое состоит из всех строк в ссылочной таблице. По умолчанию "All", поэтому в формуле "#All" представляет все строки в ссылочной таблице. |
| [GetTableRowTypeOfTotals](./gettablerowtypeoftotals/) | Получает типовое имя строк таблицы, которое состоит из итоговой строки ссылочной таблицы. По умолчанию "Totals", поэтому в формуле "#Totals" представляет итоговую строку ссылочной таблицы. |
| [GetTableRowTypeOfCurrent](./gettablerowtypeofcurrent/) | Получает типовое имя строк таблицы, которое состоит из текущей строки в ссылочной таблице. По умолчанию "This Row", поэтому в формуле "#This Row" представляет текущую строку в ссылочной таблице. |
| [GetErrorValueString](./geterrorvaluestring/) | Получает строковое значение отображения для ошибочного значения ячейки. |
| [GetBooleanValueString](./getbooleanvaluestring/) | Получает строковое значение отображения для логического значения ячейки. |
| [GetLocalFunctionName](./getlocalfunctionname/) | Получает зависящее от локали имя функции в соответствии с заданным стандартным именем функции. |
| [GetStandardFunctionName](./getstandardfunctionname/) | Получает стандартное имя функции в соответствии с заданным зависящим от локали именем функции. |
| [GetLocalBuiltInName](./getlocalbuiltinname/) | Получает зависящий от локали текст для встроенного имени в соответствии с заданным стандартным текстом. |
| [GetStandardBuiltInName](./getstandardbuiltinname/) | Получает стандартный текст встроенного имени в соответствии с заданным зависящим от локали текстом. |
| [GetListSeparator](./getlistseparator/) | Получает разделитель для списка, параметров функции и т.д. |
| [GetRowSeparatorOfFormulaArray](./getrowseparatorofformulaarray/) | Получает разделитель для строк в массивных данных в формуле. |
| [GetColumnSeparatorOfFormulaArray](./getcolumnseparatorofformulaarray/) | Получает разделитель для элементов в строковых данных массива в формуле. |
| [GetStandardHeaderFooterFontStyleName](./getstandardheaderfooterfontstylename/) | Получает стандартное английское название стиля шрифта (Regular, Bold, Italic) для Header/Footer в соответствии с указанным локализованным названием стиля шрифта. |
| [GetCommentTitleName](./getcommenttitlename/) | Получает название заголовка комментария, зависящее от локали, в соответствии с типом заголовка комментария. |
| [Compare](./compare/) | Сравнивает два строковых значения в соответствии с определёнными правилами сортировки. |
