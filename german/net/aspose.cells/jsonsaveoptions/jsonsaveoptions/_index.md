---
title: "JsonSaveOptions.JsonSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonSaveOptions-Konstruktor. Erstellt Optionen zum Speichern einer JSON-Datei"
type: docs
url: /de/net/aspose.cells/jsonsaveoptions/jsonsaveoptions/
---
## JsonSaveOptions constructor

Erstellt Optionen zum Speichern einer JSON‑Datei.

```csharp
public JsonSaveOptions()
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Beispieldaten zum Exportieren als JSON
            workbook.Worksheets[0].Cells["A1"].PutValue("Name");
            workbook.Worksheets[0].Cells["B1"].PutValue("Age");
            workbook.Worksheets[0].Cells["A2"].PutValue("John");
            workbook.Worksheets[0].Cells["B2"].PutValue(30);
            
            // JsonSaveOptions mit dem Konstruktor initialisieren
            JsonSaveOptions options = new JsonSaveOptions();
            
            // JSON-Exportoptionen festlegen
            options.ExportNestedStructure = true;
            options.SkipEmptyRows = true;
            options.ValidateMergedAreas = true;
            
            // Arbeitsmappe mit JSON-Optionen speichern
            string outputPath = "output.json";
            workbook.Save(outputPath, options);
            
            Console.WriteLine("JSON file saved successfully with options.");
        }
    }
}
```

### Siehe auch

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


