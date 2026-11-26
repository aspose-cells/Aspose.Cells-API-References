---
title: "ImportTableOptions.ColumnIndexes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImportTableOptions. Получает или задает столбцы, начиная с 0, для импорта из источника данных. null означает, что должны быть импортированы все столбцы."
type: docs
url: /ru/net/aspose.cells/importtableoptions/columnindexes/
---
## ImportTableOptions.ColumnIndexes property

Получает или задаёт столбцы (нумерация с нуля) для импорта из источника данных. null означает, что следует импортировать все столбцы.

```csharp
public int[] ColumnIndexes { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyColumnIndexesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать пример DataTable
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            // Добавьте примерные данные
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);
            dataTable.Rows.Add(3, "Product C", 39.99m);

            // Установите параметры импорта, чтобы импортировать только столбцы с индексами 0 и 2 (ID и Price).
            ImportTableOptions options = new ImportTableOptions();
            options.ColumnIndexes = new int[] { 0, 2 };
            options.IsFieldNameShown = true;

            // Импортировать данные с указанными индексами столбцов.
            worksheet.Cells.ImportData(dataTable, 0, 0, options);

            // Сохраните книгу
            workbook.Save("ColumnIndexesDemo.xlsx");
        }
    }
}
```

### См. также

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


