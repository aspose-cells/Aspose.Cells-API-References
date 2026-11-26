---
title: "SqlScriptSaveOptions.AddBlankLineBetweenRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SqlScriptSaveOptions. Вставлять пустую строку между каждым набором данных"
type: docs
url: /ru/net/aspose.cells.saving/sqlscriptsaveoptions/addblanklinebetweenrows/
---
## SqlScriptSaveOptions.AddBlankLineBetweenRows property

Вставьте пустую строку между каждым набором данных.

```csharp
public bool AddBlankLineBetweenRows { get; set; }
```

### Примечания

Если [`Separator`](../separator/) равен '\n', лучше установить это свойство в true, чтобы повысить читаемость.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyAddBlankLineBetweenRowsDemo
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
            SqlScriptSaveOptions options = new SqlScriptSaveOptions
            {
                OperatorType = SqlScriptOperatorType.Insert,
                TableName = "Employees",
                IdName = "ID",
                AddBlankLineBetweenRows = true,
                CreateTable = true
            };

            // Сохранить в поток памяти и получить SQL‑скрипт в виде строки
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, options);
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string sqlScript = reader.ReadToEnd();
                    Console.WriteLine("SQL script generated with blank lines between rows:");
                    Console.WriteLine(sqlScript);
                }
            }
        }
    }
}
```

### См. также

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


