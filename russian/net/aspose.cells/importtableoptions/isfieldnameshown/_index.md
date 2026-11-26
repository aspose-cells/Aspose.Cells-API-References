---
title: "ImportTableOptions.IsFieldNameShown"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImportTableOptions. Указывает, следует ли импортировать имя поля"
type: docs
url: /ru/net/aspose.cells/importtableoptions/isfieldnameshown/
---
## ImportTableOptions.IsFieldNameShown property

Указывает, следует ли импортировать имя поля.

```csharp
public bool IsFieldNameShown { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyIsFieldNameShownDemo
    {
        public static void Run()
        {
            // Создать примерный DataTable
            DataTable table = new DataTable();
            table.Columns.Add("ID");
            table.Columns.Add("Product");
            
            // Добавьте примерные данные
            table.Rows.Add(1, "Laptop");
            table.Rows.Add(2, "Smartphone");
            table.Rows.Add(3, "Tablet");

            // Создайте рабочую книгу и импортируйте данные с отображением имён полей
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;  // Show field names
            options.InsertRows = true;       // Insert new rows
            
            // Импортировать данные, начиная с строки 5, столбца 0
            cells.ImportData(table, 5, 0, options);
            
            // Сохраните книгу
            workbook.Save("ImportDataWithFieldNames.xlsx");
        }
    }
}
```

### См. также

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


