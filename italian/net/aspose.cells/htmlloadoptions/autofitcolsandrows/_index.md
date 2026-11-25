---
title: "HtmlLoadOptions.AutoFitColsAndRows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlLoadOptions. Indica se adattare automaticamente colonne e righe. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmlloadoptions/autofitcolsandrows/
---
## HtmlLoadOptions.AutoFitColsAndRows property

Indica se adattare automaticamente colonne e righe. Il valore predefinito è false.

```csharp
public bool AutoFitColsAndRows { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyAutoFitColsAndRowsDemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            
            // Abilita l'adattamento automatico di colonne e righe
            loadOptions.AutoFitColsAndRows = true;
            
            // Carica il file HTML con le opzioni specificate
            Workbook workbook = new Workbook("example.html", loadOptions);
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // L'adattamento automatico di colonne e righe verrà applicato durante il caricamento
            Console.WriteLine("Columns and rows have been auto-fitted during HTML import.");
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


