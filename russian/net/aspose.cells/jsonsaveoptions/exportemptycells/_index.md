---
title: "JsonSaveOptions.ExportEmptyCells"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonSaveOptions. Указывает, экспортировать ли пустые ячейки как null"
type: docs
url: /ru/net/aspose.cells/jsonsaveoptions/exportemptycells/
---
## JsonSaveOptions.ExportEmptyCells property

Указывает, экспортировать ли пустые ячейки как null.

```csharp
public bool ExportEmptyCells { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportEmptyCellsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить данные с некоторыми пустыми ячейками
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue(2.99); // B2 is intentionally left empty

            // Создать JsonSaveOptions с ExportEmptyCells, установленным в false
            JsonSaveOptions options = new JsonSaveOptions
            {
                ExportEmptyCells = false
            };

            // Сохранить в JSON — пустые ячейки будут пропущены
            workbook.Save("output_skip_empty.json", options);

            // Изменить ExportEmptyCells на true
            options.ExportEmptyCells = true;

            // Сохранить снова — пустые ячейки будут включены
            workbook.Save("output_include_empty.json", options);
        }
    }
}
```

### См. также

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


