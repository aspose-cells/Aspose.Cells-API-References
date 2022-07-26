---
title: GlobalizationSettings
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет параметры глобализации.
type: docs
weight: 3620
url: /ru/net/aspose.cells/globalizationsettings/
---
## GlobalizationSettings class

Представляет параметры глобализации.

```csharp
public class GlobalizationSettings : AbstractGlobalizationSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GlobalizationSettings](globalizationsettings)() | Конструктор по умолчанию. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings) { get; set; } | Получает или задает диаграмму этого[`ChartGlobalizationSettings`](../../aspose.cells.charts/chartglobalizationsettings) |
| virtual [ColumnSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/columnseparatorofformulaarray) { get; } | Получает разделитель элементов в данных строки массива в формуле. |
| virtual [ListSeparator](../../aspose.cells/globalizationsettings/listseparator) { get; } | Получает разделитель для списка, параметров функции и т. д. |
| virtual [RowSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/rowseparatorofformulaarray) { get; } | Получает разделитель строк в данных массива в формуле. |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [Compare](../../aspose.cells/abstractglobalizationsettings/compare)(string, string, bool) | Сравнивает два строковых значения в соответствии с определенными правилами сопоставления. |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname)() | Получает имя метки «(Все)» в сводной таблице. |
| virtual [GetBooleanValueString](../../aspose.cells/globalizationsettings/getbooleanvaluestring)(bool) | Получает отображаемое строковое значение для логического значения ячейки |
| virtual [GetCollationKey](../../aspose.cells/abstractglobalizationsettings/getcollationkey)(string, bool) | Преобразует строку в сопоставимый объект в соответствии с определенными правилами сортировки. |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable)() | Получает имя метки «Метки столбцов» в сводной таблице. |
| virtual [GetCommentTitleName](../../aspose.cells/globalizationsettings/getcommenttitlename)(CommentTitleType) | Получает зависящее от локали название заголовка комментария в соответствии с типом заголовка комментария. |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname)() | Получает имя метки "(пусто)" в сводной таблице. |
| virtual [GetErrorValueString](../../aspose.cells/globalizationsettings/geterrorvaluestring)(string) | Получает отображаемое строковое значение для ошибки ячейки value |
| virtual [GetGrandTotalName](../../aspose.cells/globalizationsettings/getgrandtotalname)(ConsolidationFunction) | Получает общее имя функции. |
| virtual [GetLocalBuiltInName](../../aspose.cells/globalizationsettings/getlocalbuiltinname)(string) | Получает зависящий от локали текст для встроенного имени в соответствии с заданным стандартным текстом. |
| virtual [GetLocalFunctionName](../../aspose.cells/globalizationsettings/getlocalfunctionname)(string) | Получает имя функции, зависящее от локали, в соответствии с заданным стандартным именем функции. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname)() | Получает имя метки «(Несколько элементов)» в сводной таблице. |
| virtual [GetOtherName](../../aspose.cells/globalizationsettings/getothername)() | Получает имя меток «Другие» для круговых диаграмм. |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname)() | Получает имя метки «Общая сумма» в сводной таблице. |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname)() | Получает имя метки «Итого» в сводной таблице. Этот метод необходимо переопределить, если сводная таблица содержит два или более сводных полей в области данных. |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable)() | Получает имя защиты в сводной таблице. |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable)() | Получает имя метки «Метки строк» в сводной таблице. |
| virtual [GetStandardBuiltInName](../../aspose.cells/globalizationsettings/getstandardbuiltinname)(string) | Получает стандартный текст встроенного имени в соответствии с заданным текстом, зависящим от языкового стандарта. |
| virtual [GetStandardFunctionName](../../aspose.cells/globalizationsettings/getstandardfunctionname)(string) | Получает стандартное имя функции в соответствии с заданным именем функции, зависящим от языкового стандарта. |
| virtual [GetStandardHeaderFooterFontStyleName](../../aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename)(string) | Получает имя стандартного английского стиля шрифта (обычный, полужирный, курсив) для верхнего/нижнего колонтитула в соответствии с заданным именем стиля шрифта локали. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname)(PivotFieldSubtotalType) | Получает имя[`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype) введите сводную таблицу. |
| virtual [GetTableRowTypeOfAll](../../aspose.cells/globalizationsettings/gettablerowtypeofall)() | Получает имя типа строк таблицы, которые состоят из всех строк в таблице, на которую ссылаются. |
| virtual [GetTableRowTypeOfCurrent](../../aspose.cells/globalizationsettings/gettablerowtypeofcurrent)() | Получает имя типа строк таблицы, которые состоят из текущей строки в ссылочной таблице. По умолчанию используется «Эта строка», поэтому в формуле «#Эта строка» представляет текущую строку в ссылочной таблице. |
| virtual [GetTableRowTypeOfData](../../aspose.cells/globalizationsettings/gettablerowtypeofdata)() | Получает имя типа строк таблицы, которые состоят из области данных таблицы, на которую ссылаются. По умолчанию используется значение «Данные», поэтому в формуле «#Данные» представляет область данных таблицы. |
| virtual [GetTableRowTypeOfHeaders](../../aspose.cells/globalizationsettings/gettablerowtypeofheaders)() | Получает имя типа строк таблицы, состоящих из заголовка таблицы. По умолчанию используется "Заголовки", поэтому в формуле "#Заголовки" представляет заголовок таблицы. |
| virtual [GetTableRowTypeOfTotals](../../aspose.cells/globalizationsettings/gettablerowtypeoftotals)() | Получает имя типа строк таблицы, состоящих из итоговой строки таблицы, на которую ссылаются. |
| virtual [GetTotalName](../../aspose.cells/globalizationsettings/gettotalname)(ConsolidationFunction) | Получает общее имя функции. |

### Смотрите также

* class [AbstractGlobalizationSettings](../abstractglobalizationsettings)
* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
