---
title: "JsonSaveOptions.ExportNestedStructure"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonSaveOptions. Esportata come struttura Json gerarchica padre-figlio"
type: docs
url: /it/net/aspose.cells/jsonsaveoptions/exportnestedstructure/
---
## JsonSaveOptions.ExportNestedStructure property

Esportato come struttura JSON gerarchica padre-figlio.

```csharp
public bool ExportNestedStructure { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportNestedStructureDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio con dati nidificati
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea una struttura di dati nidificata
            worksheet.Cells["A1"].PutValue("Parent");
            worksheet.Cells["B1"].PutValue("Child");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Fruits");
            worksheet.Cells["B3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Vegetables");
            worksheet.Cells["B4"].PutValue("Carrot");

            // Configura le opzioni di salvataggio JSON con ExportNestedStructure
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportNestedStructure = true;
            saveOptions.AlwaysExportAsJsonObject = true;

            // Salva con struttura nidificata
            string outputPath = "output_nested.json";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("Workbook exported to JSON with nested structure. Output: " + outputPath);
        }
    }
}
```

### Vedi anche

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


