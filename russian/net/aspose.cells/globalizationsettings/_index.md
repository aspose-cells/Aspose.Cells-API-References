---
title: "Класс GlobalizationSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GlobalizationSettings. Представляет настройки глобализации"
type: docs
url: /ru/net/aspose.cells/globalizationsettings/
---
## GlobalizationSettings class

Представляет настройки глобализации.

```csharp
public class GlobalizationSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings/) { get; set; } | Получает или задаёт настройки глобализации для диаграммы. |
| virtual [ColumnSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/columnseparatorofformulaarray/) { get; } | Получает разделитель для элементов в строковых данных массива в формуле. |
| virtual [ListSeparator](../../aspose.cells/globalizationsettings/listseparator/) { get; } | Получает разделитель для списка, параметров функции и т.д. |
| [PivotSettings](../../aspose.cells/globalizationsettings/pivotsettings/) { get; set; } | Получает или задаёт настройки глобализации для сводной таблицы. |
| virtual [RowSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/rowseparatorofformulaarray/) { get; } | Получает разделитель для строк в массивных данных в формуле. |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [Compare](../../aspose.cells/globalizationsettings/compare/)(string, string, bool) | Сравнивает два строковых значения в соответствии с определёнными правилами сортировки. |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname/)() | (**Obsolete.**) Получает имя метки "(All)" в PivotTable. |
| virtual [GetBooleanValueString](../../aspose.cells/globalizationsettings/getbooleanvaluestring/)(bool) | Получает отображаемое строковое значение логического значения ячейки. |
| virtual [GetCollationKey](../../aspose.cells/globalizationsettings/getcollationkey/)(string, bool) | Преобразует строку в сравнимый объект в соответствии с определёнными правилами сортировки. |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/)() | (**Obsolete.**) Получает имя метки "Column Labels" в PivotTable. |
| virtual [GetCommentTitleName](../../aspose.cells/globalizationsettings/getcommenttitlename/)(CommentTitleType) | Получает название заголовка комментария, зависящее от локали, в соответствии с типом заголовка комментария. |
| virtual [GetDataFieldHeaderNameOfPivotTable](../../aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/)() | (**Obsolete.**) Получает имя заголовка поля области значений в сводной таблице. |
| virtual [GetDefaultSheetName](../../aspose.cells/globalizationsettings/getdefaultsheetname/)() | Получает имя листа по умолчанию для автоматического добавления листа. По умолчанию "Sheet". |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname/)() | (**Obsolete.**) Получает имя метки "(blank)" в сводной таблице. |
| virtual [GetErrorValueString](../../aspose.cells/globalizationsettings/geterrorvaluestring/)(string) | Получает отображаемое строковое значение ошибки ячейки. |
| virtual [GetGrandTotalName](../../aspose.cells/globalizationsettings/getgrandtotalname/)(ConsolidationFunction) | Получает название общего итога функции. |
| virtual [GetLocalBuiltInName](../../aspose.cells/globalizationsettings/getlocalbuiltinname/)(string) | Получает текст встроенного имени, зависящий от локали, в соответствии с заданным стандартным текстом. |
| virtual [GetLocalFunctionName](../../aspose.cells/globalizationsettings/getlocalfunctionname/)(string) | Получает название функции, зависящее от локали, в соответствии с заданным стандартным названием функции. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname/)() | (**Obsolete.**) Получает имя метки "(Multiple Items)" в сводной таблице. |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname/)() | (**Obsolete.**) Получает имя метки "Grand Total" в сводной таблице. |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname/)() | (**Obsolete.**) Получает имя метки "Total" в сводной таблице. Необходимо переопределить этот метод, когда в сводной таблице в области данных содержится два или более поля PivotFields. |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable/)() | (**Obsolete.**) Получает имя защиты в сводной таблице. |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/)() | (**Obsolete.**) Получает имя метки "Row Labels" в сводной таблице. |
| virtual [GetStandardBuiltInName](../../aspose.cells/globalizationsettings/getstandardbuiltinname/)(string) | Получает стандартный текст встроенного имени в соответствии с заданным текстом, зависящим от локали. |
| virtual [GetStandardFunctionName](../../aspose.cells/globalizationsettings/getstandardfunctionname/)(string) | Получает стандартное название функции в соответствии с заданным названием функции, зависящим от локали. |
| virtual [GetStandardHeaderFooterFontStyleName](../../aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename/)(string) | Получает стандартное английское название стиля шрифта (Regular, Bold, Italic) для верхнего/нижнего колонтитула в соответствии с заданным названием стиля шрифта локали. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname/)(PivotFieldSubtotalType) | (**Obsolete.**) Получает имя типа [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) в сводной таблице. |
| virtual [GetTableRowTypeOfAll](../../aspose.cells/globalizationsettings/gettablerowtypeofall/)() | Получает название типа строк таблицы, которые состоят из всех строк в ссылочной таблице. По умолчанию "All", поэтому в формуле "#All" представляет все строки в ссылочной таблице. |
| virtual [GetTableRowTypeOfCurrent](../../aspose.cells/globalizationsettings/gettablerowtypeofcurrent/)() | Получает название типа строк таблицы, которые состоят из текущей строки в ссылочной таблице. По умолчанию "This Row", поэтому в формуле "#This Row" представляет текущую строку в ссылочной таблице. |
| virtual [GetTableRowTypeOfData](../../aspose.cells/globalizationsettings/gettablerowtypeofdata/)() | Получает название типа строк таблицы, состоящих из области данных ссылочной таблицы. По умолчанию это "Data", поэтому в формуле "#Data" представляет область данных таблицы. |
| virtual [GetTableRowTypeOfHeaders](../../aspose.cells/globalizationsettings/gettablerowtypeofheaders/)() | Получает название типа строк таблицы, состоящих из заголовка таблицы. По умолчанию это "Headers", поэтому в формуле "#Headers" представляет заголовок таблицы. |
| virtual [GetTableRowTypeOfTotals](../../aspose.cells/globalizationsettings/gettablerowtypeoftotals/)() | Получает название типа строк таблицы, которые состоят из итоговой строки ссылочной таблицы. По умолчанию "Totals", поэтому в формуле "#Totals" представляет итоговую строку ссылочной таблицы. |
| virtual [GetTotalName](../../aspose.cells/globalizationsettings/gettotalname/)(ConsolidationFunction) | Получает общее имя функции. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавьте примерные данные
            cells["A1"].PutValue("Region");
            cells["B1"].PutValue("Sales");
            cells["A2"].PutValue("North");
            cells["B2"].PutValue(1000);
            cells["A3"].PutValue("South");
            cells["B3"].PutValue(2000);
            cells["A4"].PutValue("East");
            cells["B4"].PutValue(3000);
            cells["A5"].PutValue("West");
            cells["B5"].PutValue(4000);

            // Создать и применить настройки глобализации
            GlobalizationSettings settings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // Применить подытог с пользовательской глобализацией
            CellArea area = CellArea.CreateCellArea(0, 0, 5, 1);
            cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 0 }, true, false, true);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetTotalName(ConsolidationFunction functionType)
        {
            // Настроить общее имя в зависимости от типа функции
            switch (functionType)
            {
                case ConsolidationFunction.Sum:
                    return "Custom Sum";
                case ConsolidationFunction.Count:
                    return "Custom Count";
                default:
                    return base.GetTotalName(functionType);
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


