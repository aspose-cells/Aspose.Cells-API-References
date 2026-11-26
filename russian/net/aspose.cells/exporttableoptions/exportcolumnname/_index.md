---
title: "ExportTableOptions.ExportColumnName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExportTableOptions. Указывает, экспортируются ли данные первой строки в имя столбца DataTable. Значение по умолчанию — false."
type: docs
url: /ru/net/aspose.cells/exporttableoptions/exportcolumnname/
---
## ExportTableOptions.ExportColumnName property

Указывает, экспортируются ли данные первой строки в имена столбцов DataTable. Значение по умолчанию — false.

```csharp
public bool ExportColumnName { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyExportColumnNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создать примерные данные в листе
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue(100);
            cells["B2"].PutValue("Data1");
            cells["A3"].PutValue(200);
            cells["B3"].PutValue("Data2");

            // Настроить параметры экспорта
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true; // Demonstrating ExportColumnName property
            options.IsVertical = true;
            options.Indexes = new int[] { 0, 1 }; // Export all columns

            // Экспортировать данные из листа в DataTable
            DataTable dataTable = cells.ExportDataTable(0, 0, 4, 2, options);

            // Отобразить экспортированные данные
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row["Column1"]}, {row["Column2"]}");
            }
        }
    }
}
```

### См. также

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


