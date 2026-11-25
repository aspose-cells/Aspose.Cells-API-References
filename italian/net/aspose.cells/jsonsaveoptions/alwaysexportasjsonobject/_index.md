---
title: "JsonSaveOptions.AlwaysExportAsJsonObject"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonSaveOptions. Indica se esportare sempre Excel in JSON come oggetto anche quando c'è solo un foglio di lavoro nel file"
type: docs
url: /it/net/aspose.cells/jsonsaveoptions/alwaysexportasjsonobject/
---
## JsonSaveOptions.AlwaysExportAsJsonObject property

Indica se esportare sempre Excel in JSON come oggetto, anche quando c'è solo un foglio di lavoro nel file.

```csharp
public bool AlwaysExportAsJsonObject { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyAlwaysExportAsJsonObjectDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio con due fogli di lavoro
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Imposta alcuni dati di esempio nel primo foglio di lavoro
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Value");
            cells["A2"].PutValue("Item1");
            cells["B2"].PutValue(100);

            // Configura le opzioni di salvataggio JSON
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ExportNestedStructure = true;
            saveOptions.SkipEmptyRows = true;

            // Salva in un file JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);

            // Visualizza il contenuto JSON salvato
            string jsonContent = File.ReadAllText(outputPath);
            Console.WriteLine(jsonContent);
        }
    }
}
```

### Vedi anche

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


