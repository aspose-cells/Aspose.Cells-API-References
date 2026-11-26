---
title: "SqlScriptSaveOptions.SqlScriptSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор SqlScriptSaveOptions. Создает параметры для сохранения SQL‑файла"
type: docs
url: /ru/net/aspose.cells.saving/sqlscriptsaveoptions/sqlscriptsaveoptions/
---
## SqlScriptSaveOptions constructor

Создаёт параметры для сохранения файла SQL.

```csharp
public SqlScriptSaveOptions()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            // Создайте SqlScriptSaveOptions с помощью конструктора
            SqlScriptSaveOptions options = new SqlScriptSaveOptions();
            options.OperatorType = SqlScriptOperatorType.Insert;
            options.AddBlankLineBetweenRows = true;

            // Сохранить как SQL‑скрипт
            workbook.Save("output.sql", options);
            
            // Выведите сгенерированный SQL
            Console.WriteLine("Generated SQL Script:");
            Console.WriteLine(System.IO.File.ReadAllText("output.sql"));
        }
    }
}
```

### См. также

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


