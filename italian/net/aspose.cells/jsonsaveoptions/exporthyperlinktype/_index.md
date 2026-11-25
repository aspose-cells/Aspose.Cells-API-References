---
title: "JsonSaveOptions.ExportHyperlinkType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonSaveOptions. Rappresenta il tipo di esportazione del collegamento ipertestuale in JSON"
type: docs
url: /it/net/aspose.cells/jsonsaveoptions/exporthyperlinktype/
---
## JsonSaveOptions.ExportHyperlinkType property

Rappresenta il tipo di esportazione dei collegamenti ipertestuali in JSON.

```csharp
public JsonExportHyperlinkType ExportHyperlinkType { get; set; }
```

### Osservazioni

Il valore predefinito è DisplayString;

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Json;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportHyperlinkTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un collegamento ipertestuale alla cella A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Imposta le opzioni di esportazione per JSON
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.HtmlString;
            
            // Salva la cartella di lavoro in JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);
            
            // Verifica che l'output contenga il collegamento ipertestuale
            string jsonContent = File.ReadAllText(outputPath);
            Console.WriteLine("JSON content contains hyperlink: " + 
                jsonContent.Contains("https://www.aspose.com"));
        }
    }
}
```

### Vedi anche

* enum [JsonExportHyperlinkType](../../../aspose.cells.json/jsonexporthyperlinktype/)
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


