---
title: "SqlScriptSaveOptions.CreateTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SqlScriptSaveOptions. Указывает, экспортируется ли SQL создания таблицы"
type: docs
url: /ru/net/aspose.cells.saving/sqlscriptsaveoptions/createtable/
---
## SqlScriptSaveOptions.CreateTable property

Указывает, экспортировать ли SQL создания таблицы.

```csharp
public bool CreateTable { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyCreateTableDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // Настройте параметры экспорта SQL, включив CreateTable
            SqlScriptSaveOptions options = new SqlScriptSaveOptions
            {
                CreateTable = true,
                TableName = "Employees",
                HasHeaderRow = true
            };

            // Сохранить как SQL‑скрипт
            workbook.Save("output.sql", options);
        }
    }
}
```

### См. также

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


