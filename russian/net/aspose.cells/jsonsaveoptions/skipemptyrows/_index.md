---
title: "JsonSaveOptions.SkipEmptyRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonSaveOptions. Указывает, следует ли пропускать пустые строки"
type: docs
url: /ru/net/aspose.cells/jsonsaveoptions/skipemptyrows/
---
## JsonSaveOptions.SkipEmptyRows property

Указывает, пропускать ли пустые строки.

```csharp
public bool SkipEmptyRows { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertySkipEmptyRowsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Пример данных — добавьте несколько ячеек со значениями и оставьте некоторые строки пустыми
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            // Оставьте строку 3 пустой
            worksheet.Cells["A4"].PutValue("Data3");
            worksheet.Cells["B4"].PutValue("Data4");

            // Настройте параметры сохранения JSON с SkipEmptyRows
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.SkipEmptyRows = true; // This will skip the empty row 3
            
            // Сохранить в JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("JSON saved with SkipEmptyRows=true. Empty rows were skipped.");
        }
    }
}
```

### См. также

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


