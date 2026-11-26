---
title: "SqlScriptSaveOptions.CheckAllDataForColumnType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SqlScriptSaveOptions. Проверяет все данные, чтобы определить тип данных столбцов"
type: docs
url: /ru/net/aspose.cells.saving/sqlscriptsaveoptions/checkalldataforcolumntype/
---
## SqlScriptSaveOptions.CheckAllDataForColumnType property

Проверьте все данные, чтобы определить тип данных столбцов.

```csharp
public bool CheckAllDataForColumnType { get; set; }
```

### Примечания

Значение по умолчанию — false, мы проверяем только первую строку для повышения производительности. Если это свойство истинно и столбцы содержат смешанные типы значений, тип столбцов будет текстовым.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyCheckAllDataForColumnTypeDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги с тестовыми данными
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Добавить примерные данные со смешанными типами
            sheet.Cells["A1"].PutValue("First_name");
            sheet.Cells["B1"].PutValue("Last_name");
            sheet.Cells["C1"].PutValue("age");
            sheet.Cells["D1"].PutValue("tax");
            
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["B2"].PutValue("Doe");
            sheet.Cells["C2"].PutValue(30);
            sheet.Cells["D2"].PutValue("10%");
            
            sheet.Cells["A3"].PutValue("Jane");
            sheet.Cells["B3"].PutValue("Smith");
            sheet.Cells["C3"].PutValue(25);
            sheet.Cells["D3"].PutValue(0.15);

            // Настроить параметры сохранения SQL
            SqlScriptSaveOptions sqlSaveOptions = new SqlScriptSaveOptions();
            sqlSaveOptions.OperatorType = SqlScriptOperatorType.Insert;
            sqlSaveOptions.CreateTable = true;
            sqlSaveOptions.CheckAllDataForColumnType = true; // This will examine all data to determine column types
            
            // Сохранить как SQL‑скрипт — метод Save не возвращает строку, поэтому необходимо сначала сохранить, а затем прочитать файл.
            wb.Save("output.sql", sqlSaveOptions);
            
            // Прочитать сгенерированный SQL‑скрипт
            string sqlScript = System.IO.File.ReadAllText("output.sql");
            
            Console.WriteLine("SQL Script generated:");
            Console.WriteLine(sqlScript);
        }
    }
}
```

### См. также

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


