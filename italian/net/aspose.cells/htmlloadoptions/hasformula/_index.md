---
title: "HtmlLoadOptions.HasFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlLoadOptions. Indica se il testo è una formula se inizia con"
type: docs
url: /it/net/aspose.cells/htmlloadoptions/hasformula/
---
## HtmlLoadOptions.HasFormula property

Indica se il testo è una formula se inizia con "=\".

```csharp
public bool HasFormula { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            
            // Imposta HasFormula su false per trattare le stringhe di formula come testo semplice
            loadOptions.HasFormula = false;
            
            // Crea una cartella di lavoro con file HTML e opzioni di caricamento
            Workbook workbook = new Workbook("example.html", loadOptions);
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Visualizza alcuni valori di cella per dimostrare l'importazione HTML
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("B1: " + cells["B1"].StringValue);
            
            // Salva come XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


