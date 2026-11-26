---
title: "SqlScriptSaveOptions.ExportAsString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SqlScriptSaveOptions. Указывает, экспортируются ли все данные как строковое значение"
type: docs
url: /ru/net/aspose.cells.saving/sqlscriptsaveoptions/exportasstring/
---
## SqlScriptSaveOptions.ExportAsString property

Указывает, экспортировать ли все данные как строковое значение.

```csharp
public bool ExportAsString { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");

            // Настройте параметры экспорта SQL
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                ExportAsString = true, // Demonstrating ExportAsString property
                HasHeaderRow = true
            };

            // Сохраните с включённым экспортом строк
            workbook.Save("ExportAsString_True.sql", saveOptions);

            // Измените на false и сохраните снова
            saveOptions.ExportAsString = false;
            workbook.Save("ExportAsString_False.sql", saveOptions);

            Console.WriteLine("SQL scripts saved with different ExportAsString settings.");
        }
    }
}
```

### См. также

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


