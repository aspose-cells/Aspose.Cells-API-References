---
title: "ExportTableOptions.DataTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExportTableOptions. Получает и задаёт DataTable, для которой назначается тип данных столбцов"
type: docs
url: /ru/net/aspose.cells/exporttableoptions/datatable/
---
## ExportTableOptions.DataTable property

Получает и задаёт DataTable, тип данных столбцов которого назначен.

```csharp
public DataTable DataTable { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyDataTableDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавить примерные данные в ячейки
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue(100);
            cells["B2"].PutValue("Text1");
            cells["A3"].PutValue(200);
            cells["B3"].PutValue("Text2");

            // Создать DataTable и определить столбцы
            DataTable dt = new DataTable();
            dt.Columns.Add("NumericData", typeof(double));
            dt.Columns.Add("TextData", typeof(string));

            // Настроить параметры экспорта
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            options.Indexes = new int[] { 0, 1 }; // Export both columns
            options.DataTable = dt;

            // Экспортировать данные в DataTable
            cells.ExportDataTable(0, 0, 3, 2, options);

            // Отобразить экспортированные данные
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row["NumericData"]}, {row["TextData"]}");
            }
        }
    }
}
```

### См. также

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


