---
title: "ExportTableOptions.AllowDBNull"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExportTableOptions. Это значение указывает, разрешены ли DBNull в этой таблице"
type: docs
url: /ru/net/aspose.cells/exporttableoptions/allowdbnull/
---
## ExportTableOptions.AllowDBNull property

Это значение указывает, разрешены ли DBNull в этой таблице.

```csharp
public bool AllowDBNull { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyAllowDBNullDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги с тестовыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные с некоторыми пустыми ячейками
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue(""); // Empty cell
            worksheet.Cells["B3"].PutValue(25);

            // Экспортировать с AllowDBNull = true (по умолчанию)
            ExportTableOptions options1 = new ExportTableOptions
            {
                ExportColumnName = true,
                AllowDBNull = true
            };
            
            DataTable table1 = worksheet.Cells.ExportDataTable(0, 0, 3, 2, options1);
            Console.WriteLine("With AllowDBNull=true:");
            Console.WriteLine("Row 2 Name: " + (table1.Rows[1]["Name"] == DBNull.Value ? "DBNull" : table1.Rows[1]["Name"]));

            // Экспортировать с AllowDBNull = false
            ExportTableOptions options2 = new ExportTableOptions
            {
                ExportColumnName = true,
                AllowDBNull = false
            };
            
            DataTable table2 = worksheet.Cells.ExportDataTable(0, 0, 3, 2, options2);
            Console.WriteLine("\nWith AllowDBNull=false:");
            Console.WriteLine("Row 2 Name: " + (table2.Rows[1]["Name"] == DBNull.Value ? "DBNull" : table2.Rows[1]["Name"]));
        }
    }
}
```

### См. также

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


