---
title: "JsonSaveOptions.ExportArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonSaveOptions. Получает или задает диапазон экспорта"
type: docs
url: /ru/net/aspose.cells/jsonsaveoptions/exportarea/
---
## JsonSaveOptions.ExportArea property

Получает или задает диапазон экспорта.

```csharp
public CellArea ExportArea { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить пример данных
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Настроить параметры сохранения JSON с ExportArea
            JsonSaveOptions saveOptions = new JsonSaveOptions
            {
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 }
            };

            // Сохранить с указанным диапазоном экспорта (A1:B3)
            workbook.Save("JsonExportAreaDemo.json", saveOptions);
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


