---
title: "ExportTableOptions.ExportAsString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExportTableOptions. Экспортирует строковое значение ячеек в DataTable"
type: docs
url: /ru/net/aspose.cells/exporttableoptions/exportasstring/
---
## ExportTableOptions.ExportAsString property

Экспортирует строковое значение ячеек в DataTable.

```csharp
public bool ExportAsString { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные со смешанными типами
            worksheet.Cells[0, 0].PutValue("ID");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue(1);
            worksheet.Cells[1, 1].PutValue(123.45);
            worksheet.Cells[2, 0].PutValue(2);
            worksheet.Cells[2, 1].PutValue("TextValue");

            // Создайте параметры экспорта с ExportAsString, установленным в true
            ExportTableOptions exportOptions = new ExportTableOptions
            {
                ExportColumnName = true,
                ExportAsString = true // This forces all values to be exported as strings
            };

            // Экспортировать данные в DataTable
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);

            // Отобразить типы экспортированных данных
            Console.WriteLine("Data exported with ExportAsString=true:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row[0]} ({row[0].GetType().Name}) | {row[1]} ({row[1].GetType().Name})");
            }

            // Теперь экспортировать с ExportAsString=false
            exportOptions.ExportAsString = false;
            DataTable dataTable2 = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);

            Console.WriteLine("\nData exported with ExportAsString=false:");
            foreach (DataRow row in dataTable2.Rows)
            {
                Console.WriteLine($"{row[0]} ({row[0].GetType().Name}) | {row[1]} ({row[1].GetType().Name})");
            }
        }
    }
}
```

### См. также

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


