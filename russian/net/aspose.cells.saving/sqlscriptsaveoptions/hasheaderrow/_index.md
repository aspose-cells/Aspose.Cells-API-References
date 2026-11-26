---
title: "SqlScriptSaveOptions.HasHeaderRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SqlScriptSaveOptions. Указывает, содержит ли диапазон строку заголовка"
type: docs
url: /ru/net/aspose.cells.saving/sqlscriptsaveoptions/hasheaderrow/
---
## SqlScriptSaveOptions.HasHeaderRow property

Указывает, содержит ли диапазон строку заголовка.

```csharp
public bool HasHeaderRow { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте строку заголовка и примерные данные
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Bob");

            // Настройте параметры экспорта SQL, установив HasHeaderRow=true
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                HasHeaderRow = true,
                CreateTable = true
            };

            // Сохранить как SQL‑скрипт
            workbook.Save("Employees.sql", saveOptions);

            Console.WriteLine("SQL script with header row exported successfully.");
        }
    }
}
```

### См. также

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


