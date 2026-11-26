---
title: "JsonSaveOptions.Indent"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonSaveOptions. Указывает отступ"
type: docs
url: /ru/net/aspose.cells/jsonsaveoptions/indent/
---
## JsonSaveOptions.Indent property

Указывает отступ.

```csharp
public string Indent { get; set; }
```

### Примечания

Если отступ равен null или пуст, экспортированный json не будет отформатирован.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyIndentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Настройте параметры сохранения JSON с отступом
            JsonSaveOptions saveOptions = new JsonSaveOptions
            {
                Indent = "    ", // 4 spaces for indentation
                ExportArea = new CellArea { StartRow = 0, EndRow = 3, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true
            };

            // Сохранить с отформатированным JSON с отступом
            workbook.Save("IndentedJsonOutput.json", saveOptions);
        }
    }
}
```

### См. также

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


