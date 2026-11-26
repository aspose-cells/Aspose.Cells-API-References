---
title: "SqlScriptSaveOptions.PrimaryKey"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SqlScriptSaveOptions. Представляет, какой столбец является первичным ключом таблицы данных"
type: docs
url: /ru/net/aspose.cells.saving/sqlscriptsaveoptions/primarykey/
---
## SqlScriptSaveOptions.PrimaryKey property

Представляет, какой столбец является первичным ключом таблицы данных.

```csharp
public int PrimaryKey { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyPrimaryKeyDemo
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

            // Настройте параметры экспорта SQL, установив PrimaryKey в первый столбец (0)
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                PrimaryKey = 0,
                TableName = "Employees",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Сохранить как SQL‑скрипт
            workbook.Save("EmployeesExport.sql", saveOptions);

            Console.WriteLine("SQL script exported with PrimaryKey set to column 0 (ID)");
        }
    }
}
```

### См. также

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


