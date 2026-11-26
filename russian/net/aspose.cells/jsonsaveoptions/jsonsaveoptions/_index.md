---
title: "JsonSaveOptions.JsonSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор JsonSaveOptions. Создаёт параметры для сохранения json‑файла"
type: docs
url: /ru/net/aspose.cells/jsonsaveoptions/jsonsaveoptions/
---
## JsonSaveOptions constructor

Создаёт параметры для сохранения файла JSON.

```csharp
public JsonSaveOptions()
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Пример данных для экспорта в JSON
            workbook.Worksheets[0].Cells["A1"].PutValue("Name");
            workbook.Worksheets[0].Cells["B1"].PutValue("Age");
            workbook.Worksheets[0].Cells["A2"].PutValue("John");
            workbook.Worksheets[0].Cells["B2"].PutValue(30);
            
            // Инициализируйте JsonSaveOptions с помощью конструктора
            JsonSaveOptions options = new JsonSaveOptions();
            
            // Установите параметры экспорта JSON
            options.ExportNestedStructure = true;
            options.SkipEmptyRows = true;
            options.ValidateMergedAreas = true;
            
            // Сохраните книгу с параметрами JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, options);
            
            Console.WriteLine("JSON file saved successfully with options.");
        }
    }
}
```

### См. также

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


