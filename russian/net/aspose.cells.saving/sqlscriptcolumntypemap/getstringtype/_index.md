---
title: "SqlScriptColumnTypeMap.GetStringType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SqlScriptColumnTypeMap. Получает тип строки в базе данных"
type: docs
url: /ru/net/aspose.cells.saving/sqlscriptcolumntypemap/getstringtype/
---
## SqlScriptColumnTypeMap.GetStringType method

Получает строковый тип в базе данных.

```csharp
public virtual string GetStringType()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptColumnTypeMapMethodGetStringTypeDemo
    {
        public static void Run()
        {
            // Создайте экземпляр SqlScriptColumnTypeMap
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // Получить и отобразить тип строки по умолчанию
            string stringType = columnTypeMap.GetStringType();
            Console.WriteLine("Default String Type: " + stringType);

            // Создать простой рабочий лист со строковыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John Doe");

            // Сохранить с параметрами SQL‑скрипта, используя карту типов
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };
            
            workbook.Save("SqlScriptOutput.sql", saveOptions);
            Console.WriteLine("SQL script saved with string type: " + stringType);
        }
    }
}
```

### См. также

* class [SqlScriptColumnTypeMap](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


