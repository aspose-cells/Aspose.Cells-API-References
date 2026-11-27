---
title: "JsonLoadOptions.JsonLoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonLoadOptions-konstruktor. Skapar ett alternativ för att läsa in filen"
type: docs
url: /sv/net/aspose.cells/jsonloadoptions/jsonloadoptions/
---
## JsonLoadOptions constructor

Skapar alternativ för att läsa in filen.

```csharp
public JsonLoadOptions()
```

### Exempel

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
            // Käll- och utdatamappar
            string sourceDir = "SourceDir/";
            string outputDir = "OutputDir/";
            
            // Skapa JsonLoadOptions med hjälp av konstruktorn
            JsonLoadOptions loadOptions = new JsonLoadOptions();
            loadOptions.KeptSchema = true;

            // Läs in JSON-fil med alternativ
            Workbook workbook = new Workbook(sourceDir + "example.json", loadOptions);
            
            // Spara som Excel-fil
            workbook.Save(outputDir + "example.xlsx");

            // Spara tillbaka till JSON med JsonSaveOptions
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

### Se även

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


