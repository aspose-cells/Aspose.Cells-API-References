---
title: "ExportTableOptions.PlotVisibleRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExportTableOptions. Экспортирует только видимые строки"
type: docs
url: /ru/net/aspose.cells/exporttableoptions/plotvisiblerows/
---
## ExportTableOptions.PlotVisibleRows property

Экспортирует только видимые строки.

```csharp
public bool PlotVisibleRows { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyPlotVisibleRowsDemo
    {
        public static void Run()
        {
            // Создайте книгу и откройте первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создайте примерные данные в листе
            cells["A1"].PutValue("Column1");
            cells["A2"].PutValue(10);
            cells["A3"].PutValue(20);
            cells["A4"].PutValue(30);

            // Скройте строку 3 (индекс 2), содержащую значение 20
            worksheet.Cells.HideRow(2);

            // Создайте DataTable для экспорта
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Column1", typeof(int));

            // Настройте параметры экспорта
            ExportTableOptions options = new ExportTableOptions();
            options.PlotVisibleRows = true; // Only export visible rows
            options.ExportColumnName = true;
            options.DataTable = dataTable;

            // Экспортировать данные (должна быть пропущена скрытая строка)
            cells.ExportDataTable(0, 0, 4, 1, options);

            // Отобразить экспортированные данные
            Console.WriteLine("Exported Data (PlotVisibleRows=true):");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine(row["Column1"]);
            }
        }
    }
}
```

### См. также

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


