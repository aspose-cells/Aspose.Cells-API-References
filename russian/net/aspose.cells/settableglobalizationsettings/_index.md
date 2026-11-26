---
title: "Класс SettableGlobalizationSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.SettableGlobalizationSettings. Реализация GlobalizationSettings, позволяющая пользователю задавать/изменять предопределённые тексты"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/
---
## SettableGlobalizationSettings class

Реализация GlobalizationSettings, позволяющая пользователю задавать/изменять предопределённые тексты.

```csharp
public class SettableGlobalizationSettings : GlobalizationSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [SettableGlobalizationSettings](settableglobalizationsettings/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings/) { get; set; } | Получает или задает параметры глобализации для Chart.(Наследовано от [`GlobalizationSettings`](../globalizationsettings/).) |
| override [ColumnSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/columnseparatorofformulaarray/) { get; } | Получает разделитель для элементов в строковых данных массива в формуле. |
| override [ListSeparator](../../aspose.cells/settableglobalizationsettings/listseparator/) { get; } | Получает разделитель для списка, параметров функции и т.д. |
| [PivotSettings](../../aspose.cells/globalizationsettings/pivotsettings/) { get; set; } | Получает или задает параметры глобализации для сводной таблицы.(Наследовано от [`GlobalizationSettings`](../globalizationsettings/).) |
| override [RowSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/rowseparatorofformulaarray/) { get; } | Получает разделитель для строк в массивных данных в формуле. |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [Compare](../../aspose.cells/globalizationsettings/compare/)(string, string, bool) | Сравнивает два строковых значения согласно определённым правилам сортировки.(Наследовано от [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname/)() | (**Obsolete.**) Получает имя метки "(All)" в сводной таблице. (Наследовано от [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetBooleanValueString](../../aspose.cells/settableglobalizationsettings/getbooleanvaluestring/)(bool) | Получает отображаемое строковое значение логического значения ячейки. |
| virtual [GetCollationKey](../../aspose.cells/globalizationsettings/getcollationkey/)(string, bool) | Преобразует строку в сравнимый объект в соответствии с определёнными правилами сортировки. (Наследовано от [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/)() | (**Obsolete.**) Получает имя метки "Column Labels" в сводной таблице. (Наследовано от [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetCommentTitleName](../../aspose.cells/settableglobalizationsettings/getcommenttitlename/)(CommentTitleType) | Получает название заголовка комментария, зависящее от локали, в соответствии с типом заголовка комментария. |
| virtual [GetDataFieldHeaderNameOfPivotTable](../../aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/)() | (**Obsolete.**) Получает имя заголовка поля области значений в сводной таблице. (Наследовано от [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetDefaultSheetName](../../aspose.cells/globalizationsettings/getdefaultsheetname/)() | Получает имя листа по умолчанию для автоматического добавления листа. По умолчанию это "Sheet". (Наследовано от [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname/)() | (**Obsolete.**) Получает имя метки "(blank)" в сводной таблице. (Наследовано от [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetErrorValueString](../../aspose.cells/settableglobalizationsettings/geterrorvaluestring/)(string) | Получает отображаемое строковое значение ошибки ячейки. |
| override [GetGrandTotalName](../../aspose.cells/settableglobalizationsettings/getgrandtotalname/)(ConsolidationFunction) | Получает название общего итога функции. |
| override [GetLocalBuiltInName](../../aspose.cells/settableglobalizationsettings/getlocalbuiltinname/)(string) | Получает текст встроенного имени, зависящий от локали, в соответствии с заданным стандартным текстом. |
| override [GetLocalFunctionName](../../aspose.cells/settableglobalizationsettings/getlocalfunctionname/)(string) | Получает название функции, зависящее от локали, в соответствии с заданным стандартным названием функции. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname/)() | (**Obsolete.**) Получает имя метки "(Multiple Items)" в сводной таблице. (Наследовано от [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname/)() | (**Obsolete.**) Получает имя метки "Grand Total" в сводной таблице. (Наследовано от [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname/)() | (**Obsolete.**) Получает имя метки "Total" в сводной таблице. Необходимо переопределить этот метод, когда сводная таблица содержит два или более полей PivotFields в области данных. (Наследовано от [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable/)() | (**Obsolete.**) Получает название защиты в сводной таблице. (Наследовано от [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/)() | (**Obsolete.**) Получает имя метки "Row Labels" в сводной таблице. (Наследовано от [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetStandardBuiltInName](../../aspose.cells/settableglobalizationsettings/getstandardbuiltinname/)(string) | Получает стандартный текст встроенного имени в соответствии с заданным текстом, зависящим от локали. |
| override [GetStandardFunctionName](../../aspose.cells/settableglobalizationsettings/getstandardfunctionname/)(string) | Получает стандартное название функции в соответствии с заданным названием функции, зависящим от локали. |
| override [GetStandardHeaderFooterFontStyleName](../../aspose.cells/settableglobalizationsettings/getstandardheaderfooterfontstylename/)(string) | Получает стандартное английское название стиля шрифта (Regular, Bold, Italic) для верхнего/нижнего колонтитула в соответствии с заданным названием стиля шрифта локали. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname/)(PivotFieldSubtotalType) | (**Obsolete.**) Получает имя типа [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) в сводной таблице. (Наследовано от [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetTableRowTypeOfAll](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofall/)() | Получает название типа строк таблицы, состоящих из всех строк в ссылочной таблице. |
| override [GetTableRowTypeOfCurrent](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofcurrent/)() | Получает название типа строк таблицы, состоящих из текущей строки в ссылочной таблице. |
| override [GetTableRowTypeOfData](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofdata/)() | Получает название типа строк таблицы, состоящих из области данных ссылочной таблицы. По умолчанию это "Data", поэтому в формуле "#Data" представляет область данных таблицы. |
| override [GetTableRowTypeOfHeaders](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofheaders/)() | Получает название типа строк таблицы, состоящих из заголовка таблицы. По умолчанию это "Headers", поэтому в формуле "#Headers" представляет заголовок таблицы. |
| override [GetTableRowTypeOfTotals](../../aspose.cells/settableglobalizationsettings/gettablerowtypeoftotals/)() | Получает имя типа строк таблицы, которые состоят из итоговой строки ссылочной таблицы. |
| override [GetTotalName](../../aspose.cells/settableglobalizationsettings/gettotalname/)(ConsolidationFunction) | Получает полное имя конкретной функции. |
| [SetBooleanValueString](../../aspose.cells/settableglobalizationsettings/setbooleanvaluestring/)(bool, string) | Устанавливает строковое значение отображения для логического значения ячейки. |
| [SetColumnSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/setcolumnseparatorofformulaarray/)(char) | Устанавливает разделитель для элементов данных строки массива в формуле. |
| [SetCommentTitleName](../../aspose.cells/settableglobalizationsettings/setcommenttitlename/)(CommentTitleType, string) | Получает название заголовка комментария, зависящее от локали, в соответствии с типом заголовка комментария. |
| [SetGrandTotalName](../../aspose.cells/settableglobalizationsettings/setgrandtotalname/)(ConsolidationFunction, string) | Устанавливает имя общего итога конкретной функции. |
| [SetListSeparator](../../aspose.cells/settableglobalizationsettings/setlistseparator/)(char) | Устанавливает разделитель для списка, параметров функции и т.д. |
| [SetLocalBuiltInName](../../aspose.cells/settableglobalizationsettings/setlocalbuiltinname/)(string, string, bool) | Устанавливает зависящий от локали текст для встроенного имени с заданным стандартным текстом имени. |
| [SetLocalFunctionName](../../aspose.cells/settableglobalizationsettings/setlocalfunctionname/)(string, string, bool) | Устанавливает зависящее от локали имя функции, соответствующее заданному стандартному имени функции. |
| [SetRowSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/setrowseparatorofformulaarray/)(char) | Устанавливает разделитель для строк в данных массива в формуле. |
| [SetStandardBuiltInName](../../aspose.cells/settableglobalizationsettings/setstandardbuiltinname/)(string, string, bool) | Устанавливает зависящее от локали имя функции в соответствии с заданным стандартным именем функции. |
| [SetStandardFunctionName](../../aspose.cells/settableglobalizationsettings/setstandardfunctionname/)(string, string, bool) | Устанавливает зависящее от локали имя функции в соответствии с заданным стандартным именем функции. |
| [SetStandardHeaderFooterFontStyleName](../../aspose.cells/settableglobalizationsettings/setstandardheaderfooterfontstylename/)(string, string) | Устанавливает зависящее от локали имя функции в соответствии с заданным стандартным именем функции. |
| [SetTableRowTypeOfAll](../../aspose.cells/settableglobalizationsettings/settablerowtypeofall/)(string) | Устанавливает имя типа строк таблицы, которые состоят из всех строк в ссылочной таблице. |
| [SetTableRowTypeOfCurrent](../../aspose.cells/settableglobalizationsettings/settablerowtypeofcurrent/)(string) | Устанавливает имя типа строк таблицы, которые состоят из текущей строки в ссылочной таблице. |
| [SetTableRowTypeOfData](../../aspose.cells/settableglobalizationsettings/settablerowtypeofdata/)(string) | Устанавливает имя типа строк таблицы, которые состоят из области данных ссылочной таблицы. |
| [SetTableRowTypeOfHeaders](../../aspose.cells/settableglobalizationsettings/settablerowtypeofheaders/)(string) | Устанавливает имя типа строк таблицы, которые состоят из заголовка таблицы. |
| [SetTableRowTypeOfTotals](../../aspose.cells/settableglobalizationsettings/settablerowtypeoftotals/)(string) | Устанавливает имя типа строк таблицы, которые состоят из итоговой строки ссылочной таблицы. |
| [SetTotalName](../../aspose.cells/settableglobalizationsettings/settotalname/)(ConsolidationFunction, string) | Устанавливает полное имя конкретной функции. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;

    public class CellsClassSettableGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте экземпляр SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // Установите пользовательский разделитель списка
            settings.SetListSeparator(';');

            // Установите пользовательские строки логических значений
            settings.SetBooleanValueString(true, "TRUE_CUSTOM");
            settings.SetBooleanValueString(false, "FALSE_CUSTOM");

            // Установите пользовательские имена функций
            settings.SetLocalFunctionName("SUM", "SUMME", true);
            settings.SetLocalFunctionName("AVERAGE", "MITTELWERT", true);

            // Установите пользовательские имена типов строк таблицы
            settings.SetTableRowTypeOfHeaders("HEADERS_CUSTOM");
            settings.SetTableRowTypeOfData("DATA_CUSTOM");
            settings.SetTableRowTypeOfTotals("TOTALS_CUSTOM");

            // Установите пользовательские имена заголовков комментариев
            settings.SetCommentTitleName(CommentTitleType.Comment, "COMMENT_CUSTOM");
            // Удалена строка Author, поскольку CommentTitleType не имеет такого значения перечисления
            // Если вам необходимо задать настройки, связанные с автором, следует использовать ThreadedCommentAuthor

            // Примените настройки глобализации к рабочей книге
            workbook.Settings.GlobalizationSettings = settings;

            // Продемонстрировать использование в формулах
            worksheet.Cells["A1"].Formula = "=TRUE()";
            worksheet.Cells["A2"].Formula = "=FALSE()";
            worksheet.Cells["A3"].Formula = "=SUM(1,2,3)";
            worksheet.Cells["A4"].Formula = "=AVERAGE(1,2,3)";

            // Сохраните книгу
            workbook.Save("SettableGlobalizationSettingsDemo.xlsx");
        }
    }
}
```

### См. также

* class [GlobalizationSettings](../globalizationsettings/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


