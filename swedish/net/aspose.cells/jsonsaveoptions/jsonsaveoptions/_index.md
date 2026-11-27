---
title: "JsonSaveOptions.JsonSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonSaveOptions-konstruktor. Skapar alternativ för att spara json-fil"
type: docs
url: /sv/net/aspose.cells/jsonsaveoptions/jsonsaveoptions/
---
## JsonSaveOptions constructor

Skapar alternativ för att spara JSON-fil.

```csharp
public JsonSaveOptions()
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Exempeldatat att exportera som JSON
            workbook.Worksheets[0].Cells["A1"].PutValue("Name");
            workbook.Worksheets[0].Cells["B1"].PutValue("Age");
            workbook.Worksheets[0].Cells["A2"].PutValue("John");
            workbook.Worksheets[0].Cells["B2"].PutValue(30);
            
            // Initiera JsonSaveOptions med konstruktor
            JsonSaveOptions options = new JsonSaveOptions();
            
            // Ställ in JSON-exportalternativ
            options.ExportNestedStructure = true;
            options.SkipEmptyRows = true;
            options.ValidateMergedAreas = true;
            
            // Spara arbetsbok med JSON-alternativ
            string outputPath = "output.json";
            workbook.Save(outputPath, options);
            
            Console.WriteLine("JSON file saved successfully with options.");
        }
    }
}
```

### Se även

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


