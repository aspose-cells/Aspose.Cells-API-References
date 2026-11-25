---
title: "JsonLoadOptions.JsonLoadOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore di JsonLoadOptions. Crea un'opzione per il caricamento del file"
type: docs
url: /it/net/aspose.cells/jsonloadoptions/jsonloadoptions/
---
## JsonLoadOptions constructor

Crea un'opzione per il caricamento del file.

```csharp
public JsonLoadOptions()
```

### Esempi

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
            // Directory di origine e di destinazione
            string sourceDir = "SourceDir/";
            string outputDir = "OutputDir/";
            
            // Crea JsonLoadOptions usando il costruttore
            JsonLoadOptions loadOptions = new JsonLoadOptions();
            loadOptions.KeptSchema = true;

            // Carica il file JSON con le opzioni
            Workbook workbook = new Workbook(sourceDir + "example.json", loadOptions);
            
            // Salva come file Excel
            workbook.Save(outputDir + "example.xlsx");

            // Salva nuovamente in JSON con JsonSaveOptions
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

### Vedi anche

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


