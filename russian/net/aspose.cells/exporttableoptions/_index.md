---
title: "Класс ExportTableOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ExportTableOptions. Представляет все параметры экспорта таблицы"
type: docs
url: /ru/net/aspose.cells/exporttableoptions/
---
## ExportTableOptions class

Представляет все параметры экспорта таблицы.

```csharp
public class ExportTableOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ExportTableOptions](exporttableoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AllowDBNull](../../aspose.cells/exporttableoptions/allowdbnull/) { get; set; } | Это значение указывает, разрешены ли DBNull в этой таблице. |
| [CheckMixedValueType](../../aspose.cells/exporttableoptions/checkmixedvaluetype/) { get; set; } | False: Aspose.Cells установит тип DataColumn по типу значения первой строки для повышения производительности. True: Aspose.Cells проверит, смешаны ли типы значений в столбце, перед установкой типа DataColumn, и если типы смешаны, тип DataColumn будет string. |
| [DataTable](../../aspose.cells/exporttableoptions/datatable/) { get; set; } | Получает и задаёт DataTable, тип данных столбцов которого назначен. |
| [ExportAsHtmlString](../../aspose.cells/exporttableoptions/exportashtmlstring/) { get; set; } | Экспортирует строковое значение HTML ячеек в DataTable. |
| [ExportAsString](../../aspose.cells/exporttableoptions/exportasstring/) { get; set; } | Экспортирует строковое значение ячеек в DataTable. |
| [ExportColumnName](../../aspose.cells/exporttableoptions/exportcolumnname/) { get; set; } | Указывает, экспортируются ли данные первой строки в имена столбцов DataTable. Значение по умолчанию — false. |
| [FormatStrategy](../../aspose.cells/exporttableoptions/formatstrategy/) { get; set; } | Получает и задаёт стратегию форматирования при экспорте значения как строкового. |
| [Indexes](../../aspose.cells/exporttableoptions/indexes/) { get; set; } | Индексы столбцов/строк, которые должны быть экспортированы. |
| [IsVertical](../../aspose.cells/exporttableoptions/isvertical/) { get; set; } | True, если строка в файле Workbook представляет строку в DataTable. False, если столбец в файле Workbook представляет строку в DataTable. |
| [PlotVisibleCells](../../aspose.cells/exporttableoptions/plotvisiblecells/) { get; set; } | Экспортирует только видимые ячейки. |
| [PlotVisibleColumns](../../aspose.cells/exporttableoptions/plotvisiblecolumns/) { get; set; } | Экспортирует только видимые столбцы. |
| [PlotVisibleRows](../../aspose.cells/exporttableoptions/plotvisiblerows/) { get; set; } | Экспортирует только видимые строки. |
| [RenameStrategy](../../aspose.cells/exporttableoptions/renamestrategy/) { get; set; } | Стратегия для дублирующихся имён столбцов. |
| [SkipErrorValue](../../aspose.cells/exporttableoptions/skiperrorvalue/) { get; set; } | Указывает, следует ли пропускать недопустимые значения для столбца. Например, если тип столбца decimal, значение превышает decimal.MaxValue и это свойство равно true, исключение выброшено не будет. Значение по умолчанию — false. |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [PreprocessExportedValue](../../aspose.cells/exporttableoptions/preprocessexportedvalue/)(int, int, CellValue) | Предобработать значение текущей ячейки перед экспортом. |

### Примечания

Если есть специальные требования к экспорту, например игнорирование ошибочных значений, пользователь может расширить этот класс, переопределив соответствующие API для достижения цели.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ExportTableOptionsDemo
    {
        public static void ExportTableOptionsExample()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые образцы данных в лист
            worksheet.Cells[0, 0].PutValue("Name");
            worksheet.Cells[0, 1].PutValue("Age");
            worksheet.Cells[1, 0].PutValue("John");
            worksheet.Cells[1, 1].PutValue(30);
            worksheet.Cells[2, 0].PutValue("Jane");
            worksheet.Cells[2, 1].PutValue(25);

            // Создайте экземпляр ExportTableOptions
            ExportTableOptions exportOptions = new ExportTableOptions
            {
                ExportColumnName = true,
                SkipErrorValue = true,
                PlotVisibleCells = true,
                PlotVisibleRows = true,
                PlotVisibleColumns = true,
                ExportAsString = false,
                ExportAsHtmlString = false,
                FormatStrategy = CellValueFormatStrategy.DisplayStyle,
                CheckMixedValueType = true,
                AllowDBNull = true,
                IsVertical = true,
                RenameStrategy = RenameStrategy.Digit
            };

            // Экспортируйте данные из листа в DataTable
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);

            // Отобразить экспортированные данные
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }

            // Сохраните книгу
            workbook.Save("ExportTableOptionsExample.xlsx");
            workbook.Save("ExportTableOptionsExample.pdf");
        }
    }

}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


