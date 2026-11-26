---
title: "JsonLoadOptions.JsonLoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор JsonLoadOptions. Создаёт параметры загрузки файла"
type: docs
url: /ru/net/aspose.cells/jsonloadoptions/jsonloadoptions/
---
## JsonLoadOptions constructor

Создаёт параметры загрузки файла.

```csharp
public JsonLoadOptions()
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Каталоги источника и вывода
            string sourceDir = "SourceDir/";
            string outputDir = "OutputDir/";
            
            // Создайте JsonLoadOptions с помощью конструктора
            JsonLoadOptions loadOptions = new JsonLoadOptions();
            loadOptions.KeptSchema = true;

            // Загрузите JSON-файл с параметрами
            Workbook workbook = new Workbook(sourceDir + "example.json", loadOptions);
            
            // Сохранить как файл Excel
            workbook.Save(outputDir + "example.xlsx");

            // Сохранить обратно в JSON с JsonSaveOptions
            workbook.Save(outputDir + "example_output.json", new JsonSaveOptions()
            {
                ExportNestedStructure = true,
                SkipEmptyRows = true
            });

            Console.WriteLine("JSON to Excel conversion completed successfully.");
        }
    }
}
```

### См. также

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


