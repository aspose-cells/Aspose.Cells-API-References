---
title: "SqlScriptSaveOptions.StartId"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SqlScriptSaveOptions. Получает и задаёт начальный идентификатор"
type: docs
url: /ru/net/aspose.cells.saving/sqlscriptsaveoptions/startid/
---
## SqlScriptSaveOptions.StartId property

Получает и задаёт начальный идентификатор.

```csharp
public int StartId { get; set; }
```

### Примечания

Работает только когда [`IdName`](../idname/) установлен.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyStartIdDemo
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

            // Настройте параметры экспорта SQL, установив StartId в 100
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                IdName = "ID",
                StartId = 100, // Demonstrating StartId property
                HasHeaderRow = true,
                OperatorType = SqlScriptOperatorType.Insert
            };

            // Сохранить как SQL‑скрипт
            workbook.Save("Employees_WithStartId.sql", saveOptions);
        }
    }
}
```

### См. также

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


