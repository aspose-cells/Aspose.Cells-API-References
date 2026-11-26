---
title: "ImportTableOptions.InsertRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImportTableOptions. Указывает, следует ли добавлять новые строки при импорте записей данных"
type: docs
url: /ru/net/aspose.cells/importtableoptions/insertrows/
---
## ImportTableOptions.InsertRows property

Указывает, следует ли добавлять новые строки при импорте записей данных.

```csharp
public bool InsertRows { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyInsertRowsDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создать пример таблицы данных
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            dataTable.Rows.Add(1, "Laptop", 999.99);
            dataTable.Rows.Add(2, "Monitor", 249.99);
            dataTable.Rows.Add(3, "Keyboard", 49.99);

            // Добавьте существующие данные в рабочий лист (будут смещены вниз при вставке)
            cells["A1"].PutValue("Existing Data");
            cells["A2"].PutValue(100);

            // Установите параметры импорта с InsertRows = true
            ImportTableOptions options = new ImportTableOptions();
            options.InsertRows = true; // This will insert new rows instead of overwriting
            options.IsFieldNameShown = true;

            // Импортировать данные, начиная с строки 1 (будут вставлены строки ниже существующих данных)
            cells.ImportData(dataTable, 1, 0, options);

            // Сохраните книгу
            workbook.Save("InsertRowsDemo.xlsx");
        }
    }
}
```

### См. также

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


