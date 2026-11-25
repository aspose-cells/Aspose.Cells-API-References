---
title: "JsonSaveOptions.JsonSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore JsonSaveOptions. Crea le opzioni per salvare un file json"
type: docs
url: /it/net/aspose.cells/jsonsaveoptions/jsonsaveoptions/
---
## JsonSaveOptions constructor

Crea opzioni per salvare il file JSON.

```csharp
public JsonSaveOptions()
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Dati di esempio da esportare come JSON
            workbook.Worksheets[0].Cells["A1"].PutValue("Name");
            workbook.Worksheets[0].Cells["B1"].PutValue("Age");
            workbook.Worksheets[0].Cells["A2"].PutValue("John");
            workbook.Worksheets[0].Cells["B2"].PutValue(30);
            
            // Inizializza JsonSaveOptions usando il costruttore
            JsonSaveOptions options = new JsonSaveOptions();
            
            // Imposta le opzioni di esportazione JSON
            options.ExportNestedStructure = true;
            options.SkipEmptyRows = true;
            options.ValidateMergedAreas = true;
            
            // Salva la cartella di lavoro con le opzioni JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, options);
            
            Console.WriteLine("JSON file saved successfully with options.");
        }
    }
}
```

### Vedi anche

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


