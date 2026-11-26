---
title: "SqlScriptSaveOptions.CheckIfTableExists"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SqlScriptSaveOptions. Проверяет, существует ли имя таблицы перед созданием"
type: docs
url: /ru/net/aspose.cells.saving/sqlscriptsaveoptions/checkiftableexists/
---
## SqlScriptSaveOptions.CheckIfTableExists property

Проверьте, существует ли имя таблицы перед созданием

```csharp
public bool CheckIfTableExists { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyCheckIfTableExistsDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги с тестовыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // Настроить параметры сохранения SQL
            SqlScriptSaveOptions sqlOptions = new SqlScriptSaveOptions();
            sqlOptions.CreateTable = true;
            sqlOptions.CheckIfTableExists = true;
            sqlOptions.OperatorType = SqlScriptOperatorType.Insert;

            // Сохранить в файл SQL‑скрипта
            workbook.Save("output.sql", sqlOptions);

            // Прочитать и вывести сгенерированный SQL
            string sqlScript = System.IO.File.ReadAllText("output.sql");
            Console.WriteLine("Generated SQL Script:");
            Console.WriteLine(sqlScript);
        }
    }
}
```

### См. также

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


