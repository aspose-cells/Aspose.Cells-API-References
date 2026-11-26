---
title: "ImportTableOptions.TotalColumns"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImportTableOptions. Получает или задает общее количество столбцов для импорта из источника данных. 1 означает все строки данного источника данных"
type: docs
url: /ru/net/aspose.cells/importtableoptions/totalcolumns/
---
## ImportTableOptions.TotalColumns property

Получает или задаёт общее количество столбцов для импорта из источника данных. -1 означает все строки заданного источника данных.

```csharp
public int TotalColumns { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyTotalColumnsDemo
    {
        public static void Run()
        {
            // Создать примерный DataTable
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            // Добавьте примерные данные
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);

            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите параметры импорта с TotalColumns = 2 (будут импортированы только первые 2 столбца)
            ImportTableOptions importOptions = new ImportTableOptions
            {
                IsFieldNameShown = true,
                TotalColumns = 2 // Only import first 2 columns (ID and Name)
            };

            // Импортировать данные, начиная с ячейки A1
            cells.ImportData(dataTable, 0, 0, importOptions);

            // Сохраните книгу
            workbook.Save("ImportWithTotalColumns.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Data imported with TotalColumns=2. Only first 2 columns were imported.");
        }
    }
}
```

### См. также

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


