---
title: "SqlScriptSaveOptions.ColumnTypeMap"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SqlScriptSaveOptions. Получает и задает отображение типов столбцов для разных баз данных"
type: docs
url: /ru/net/aspose.cells.saving/sqlscriptsaveoptions/columntypemap/
---
## SqlScriptSaveOptions.ColumnTypeMap property

Получает и задаёт отображение типов столбцов для разных баз данных.

```csharp
public SqlScriptColumnTypeMap ColumnTypeMap { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyColumnTypeMapDemo
    {
        public static void Run()
        {
            // Создать пользовательскую карту типов столбцов
            SqlScriptColumnTypeMap customTypeMap = new SqlScriptColumnTypeMap();
            
            // Создать параметры сохранения SQL
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                CreateTable = true,
                ColumnTypeMap = customTypeMap,
                CheckIfTableExists = true,
                ExportAsString = false
            };

            // Создать пример рабочей книги с данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить заголовки
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Salary");
            
            // Добавить строки данных
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John Smith");
            worksheet.Cells["C2"].PutValue(5000.50);
            
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane Doe");
            worksheet.Cells["C3"].PutValue(6500.75);

            // Сохранить как SQL‑скрипт
            workbook.Save("EmployeeData.sql", saveOptions);
            
            Console.WriteLine("SQL script generated successfully with custom column type mapping.");
        }
    }
}
```

### См. также

* class [SqlScriptColumnTypeMap](../../sqlscriptcolumntypemap/)
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


