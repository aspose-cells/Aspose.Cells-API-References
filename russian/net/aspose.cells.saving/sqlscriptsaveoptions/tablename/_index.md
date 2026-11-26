---
title: "SqlScriptSaveOptions.TableName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SqlScriptSaveOptions. Получает и задает имя таблицы"
type: docs
url: /ru/net/aspose.cells.saving/sqlscriptsaveoptions/tablename/
---
## SqlScriptSaveOptions.TableName property

Получает и задаёт имя таблицы.

```csharp
public string TableName { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyTableNameDemo
    {
        public static void Run()
        {
            // Создайте примерную книгу с некоторыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Настройте параметры сохранения SQL с пользовательским именем таблицы
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions();
            saveOptions.TableName = "Employees"; // Demonstrating TableName property
            saveOptions.CreateTable = true;
            saveOptions.OperatorType = SqlScriptOperatorType.Insert;

            // Сохранить как SQL‑скрипт
            workbook.Save("output.sql", saveOptions);

            Console.WriteLine("SQL Script generated with table name 'Employees'");
        }
    }
}
```

### См. также

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


