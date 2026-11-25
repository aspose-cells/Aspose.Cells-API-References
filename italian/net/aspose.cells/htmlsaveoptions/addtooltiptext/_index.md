---
title: "HtmlSaveOptions.AddTooltipText"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se aggiungere il testo del tooltip quando i dati non possono essere visualizzati completamente. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/addtooltiptext/
---
## HtmlSaveOptions.AddTooltipText property

Indica se aggiungere il testo del tooltip quando i dati non possono essere visualizzati completamente. Il valore predefinito è false.

```csharp
public bool AddTooltipText { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAddTooltipTextDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta un testo lungo che supererà la larghezza della cella
            worksheet.Cells["A1"].PutValue("This is a long text that will exceed cell width and need tooltip");
            worksheet.Cells.SetColumnWidth(0, 10); // Set narrow column width
            
            // Configura le opzioni di salvataggio HTML con tooltip
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.AddTooltipText = true;
            
            // Salva la cartella di lavoro
            string outputPath = "output_with_tooltip.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved with tooltips: " + outputPath);
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


