---
title: "SqlScriptSaveOptions.Separator"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SqlScriptSaveOptions. Получает и задает символ-разделитель SQL‑скрипта"
type: docs
url: /ru/net/aspose.cells.saving/sqlscriptsaveoptions/separator/
---
## SqlScriptSaveOptions.Separator property

Получает и задаёт символьный разделитель скрипта SQL.

```csharp
public char Separator { get; set; }
```

### Примечания

Может быть только ' ' или '\n'. Если

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertySeparatorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("John");

            // Настроить параметры сохранения SQL с пользовательским разделителем
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                Separator = ';',
                TableName = "Employees",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Сохраните с пользовательским разделителем
            workbook.Save("SqlScriptWithSeparator.sql", saveOptions);

            Console.WriteLine("SQL script saved with custom separator.");
        }
    }
}
```

### См. также

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


