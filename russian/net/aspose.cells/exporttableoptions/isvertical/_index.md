---
title: "ExportTableOptions.IsVertical"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExportTableOptions. True, если строка в файле Workbook представляет строку в DataTable. False, если столбец в файле Workbook представляет строку в DataTable."
type: docs
url: /ru/net/aspose.cells/exporttableoptions/isvertical/
---
## ExportTableOptions.IsVertical property

True, если строка в файле Workbook представляет строку в DataTable. False, если столбец в файле Workbook представляет строку в DataTable.

```csharp
public bool IsVertical { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyIsVerticalDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создать примерные данные в листе
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(25);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(30);

            // Создать DataTable
            DataTable dt = new DataTable();
            dt.Columns.Add("Column1", typeof(string));
            dt.Columns.Add("Column2", typeof(int));

            // Установить ExportTableOptions с IsVertical = true
            ExportTableOptions options = new ExportTableOptions();
            options.IsVertical = true;
            options.ExportColumnName = true;
            options.DataTable = dt;

            // Экспортировать данные вертикально
            cells.ExportDataTable(0, 0, 2, 2, options);

            // Отобразить экспортированную DataTable
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row[0]}, {row[1]}");
            }
        }
    }
}
```

### См. также

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


