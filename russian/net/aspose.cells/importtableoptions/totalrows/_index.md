---
title: "ImportTableOptions.TotalRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImportTableOptions. Получает или задает общее количество строк для импорта из источника данных. 1 означает все строки данного источника данных"
type: docs
url: /ru/net/aspose.cells/importtableoptions/totalrows/
---
## ImportTableOptions.TotalRows property

Получает или задаёт общее количество строк для импорта из источника данных. -1 означает все строки заданного источника данных.

```csharp
public int TotalRows { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyTotalRowsDemo
    {
        public static void Run()
        {
            // Создать примерный DataTable
            DataTable table = new DataTable("TestTable");
            table.Columns.Add("Column1", typeof(string));
            table.Columns.Add("Column2", typeof(int));
            
            // Добавьте примерные данные
            table.Rows.Add("Item1", 100);
            table.Rows.Add("Item2", 200);
            table.Rows.Add("Item3", 300);

            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте ImportTableOptions с установленным TotalRows = 2 (будет импортировано только первые 2 строки)
            ImportTableOptions options = new ImportTableOptions
            {
                IsFieldNameShown = true,
                TotalRows = 2 // Only import 2 rows from the DataTable
            };

            // Импортировать данные с указанными параметрами
            worksheet.Cells.ImportData(table, 0, 0, options);

            // Сохраните книгу
            workbook.Save("ImportWithTotalRows.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Data imported with TotalRows=2. Only first 2 rows were imported.");
        }
    }
}
```

### См. также

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


