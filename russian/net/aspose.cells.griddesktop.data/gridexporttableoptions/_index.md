---
title: "Класс GridExportTableOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.GridDesktop.Data.GridExportTableOptions class. Представляет все параметры экспорта таблицы."
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridexporttableoptions/
---
## GridExportTableOptions class

Представляет все параметры экспорта таблицы.

```csharp
public class GridExportTableOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GridExportTableOptions](gridexporttableoptions/)() | Конструктор GridExportTableOptions |

## Свойства

| Имя | Описание |
| --- | --- |
| [CheckMixedValueType](../../aspose.cells.griddesktop.data/gridexporttableoptions/checkmixedvaluetype/) { get; set; } | False: Aspose.Cells установит тип DataColumn по типу значения первой строки для повышения производительности. True: Aspose.Cells проверит, смешаны ли типы значений в столбце, перед установкой типа DataColumn, и если типы смешаны, тип DataColumn будет string. |
| [DataTable](../../aspose.cells.griddesktop.data/gridexporttableoptions/datatable/) { get; set; } | Получает и задаёт DataTable, тип данных столбцов которого назначен. |
| [ExportAsHtmlString](../../aspose.cells.griddesktop.data/gridexporttableoptions/exportashtmlstring/) { get; set; } | Экспортирует строковое значение HTML ячеек в DataTable. |
| [ExportAsString](../../aspose.cells.griddesktop.data/gridexporttableoptions/exportasstring/) { get; set; } | Экспортирует строковое значение ячеек в DataTable. |
| [ExportColumnName](../../aspose.cells.griddesktop.data/gridexporttableoptions/exportcolumnname/) { get; set; } | Указывает, экспортируются ли данные первой строки в имена столбцов DataTable. Значение по умолчанию — false. |
| [FormatStrategy](../../aspose.cells.griddesktop.data/gridexporttableoptions/formatstrategy/) { get; set; } | Получает и задаёт стратегию форматирования при экспорте значения как строкового. |
| [Indexes](../../aspose.cells.griddesktop.data/gridexporttableoptions/indexes/) { get; set; } | Индексы столбцов/строк, которые должны быть экспортированы. |
| [IsVertical](../../aspose.cells.griddesktop.data/gridexporttableoptions/isvertical/) { get; set; } | True, если строка в файле Workbook представляет строку в DataTable. False, если столбец в файле Workbook представляет строку в DataTable. |
| [PlotVisibleCells](../../aspose.cells.griddesktop.data/gridexporttableoptions/plotvisiblecells/) { get; set; } | Экспортирует только видимые ячейки. |
| [PlotVisibleColumns](../../aspose.cells.griddesktop.data/gridexporttableoptions/plotvisiblecolumns/) { get; set; } | Экспортирует только видимые столбцы. |
| [PlotVisibleRows](../../aspose.cells.griddesktop.data/gridexporttableoptions/plotvisiblerows/) { get; set; } | Экспортирует только видимые строки. |
| [RenameStrategy](../../aspose.cells.griddesktop.data/gridexporttableoptions/renamestrategy/) { get; set; } | Стратегия для дублирующихся имён столбцов. |
| [SkipErrorValue](../../aspose.cells.griddesktop.data/gridexporttableoptions/skiperrorvalue/) { get; set; } | Указывает, следует ли пропускать недопустимые значения для столбца. Например, если тип столбца decimal, значение превышает decimal.MaxValue и это свойство равно true, исключение выброшено не будет. Значение по умолчанию — false. |

### См. также

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


