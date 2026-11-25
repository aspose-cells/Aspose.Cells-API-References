---
title: "HtmlLoadOptions.LoadFormulas"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlLoadOptions. Indica se importare le formule se il file HTML originale contiene formule"
type: docs
url: /it/net/aspose.cells/htmlloadoptions/loadformulas/
---
## HtmlLoadOptions.LoadFormulas property

Indica se importare le formule se il file HTML originale contiene formule

```csharp
public bool LoadFormulas { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyLoadFormulasDemo
    {
        public static void Run()
        {
            // Crea un'istanza di HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Imposta LoadFormulas su true per caricare le formule da HTML
            loadOptions.LoadFormulas = true;

            // Carica un file HTML contenente formule in una Cartella di lavoro
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Visualizza la formula dalla cella A1 (se presente in HTML)
            Console.WriteLine("Formula in A1: " + worksheet.Cells["A1"].Formula);

            // Salva la cartella di lavoro in un file Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


