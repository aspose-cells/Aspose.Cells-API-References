---
title: "JsonLoadOptions.JsonLoadOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonLoadOptions-Konstruktor. Erstellt Optionen zum Laden der Datei"
type: docs
url: /de/net/aspose.cells/jsonloadoptions/jsonloadoptions/
---
## JsonLoadOptions constructor

Erstellt eine Option zum Laden der Datei.

```csharp
public JsonLoadOptions()
```

### Beispiele

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
            // Quell- und Ausgabeverzeichnisse
            string sourceDir = "SourceDir/";
            string outputDir = "OutputDir/";
            
            // JsonLoadOptions mit dem Konstruktor erstellen
            JsonLoadOptions loadOptions = new JsonLoadOptions();
            loadOptions.KeptSchema = true;

            // JSON-Datei mit Optionen laden
            Workbook workbook = new Workbook(sourceDir + "example.json", loadOptions);
            
            // Als Excel-Datei speichern
            workbook.Save(outputDir + "example.xlsx");

            // Zurück in JSON mit JsonSaveOptions speichern
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

### Siehe auch

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


