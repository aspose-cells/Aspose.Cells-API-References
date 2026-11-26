---
title: "SqlScriptSaveOptions.IdName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SqlScriptSaveOptions. Получает и задает имя столбца идентификатора"
type: docs
url: /ru/net/aspose.cells.saving/sqlscriptsaveoptions/idname/
---
## SqlScriptSaveOptions.IdName property

Получает и задаёт имя столбца идентификатора.

```csharp
public string IdName { get; set; }
```

### Примечания

Если это свойство установлено, будет вставлен столбец с автоматически увеличиваемым целочисленным значением.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyIdNameDemo
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

            // Настроить параметры экспорта SQL с IdName
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                IdName = "ID",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Сохранить как SQL‑скрипт
            workbook.Save("Employees.sql", saveOptions);

            Console.WriteLine("SQL script exported with IdName property");
        }
    }
}
```

### См. также

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


