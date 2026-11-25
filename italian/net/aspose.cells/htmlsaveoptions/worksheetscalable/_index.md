---
title: "HtmlSaveOptions.WorksheetScalable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se ingrandire o ridurre l'HTML tramite il livello di zoom del foglio di lavoro durante il salvataggio del file in HTML; il valore predefinito è false."
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/worksheetscalable/
---
## HtmlSaveOptions.WorksheetScalable property

Indica se ingrandire o ridurre l'HTML tramite il livello di zoom del foglio di lavoro durante il salvataggio del file in HTML; il valore predefinito è false.

```csharp
public bool WorksheetScalable { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyWorksheetScalableDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Imposta le opzioni di salvataggio HTML con la proprietà WorksheetScalable.
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.WorksheetScalable = true;
            
            // Salva la cartella di lavoro con le opzioni HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, options);
            
            // Verifica che l'output contenga lo stile di scaling.
            string htmlContent = File.ReadAllText(outputPath);
            Console.WriteLine("HTML contains scaling: " + htmlContent.Contains("transform: scale"));
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


