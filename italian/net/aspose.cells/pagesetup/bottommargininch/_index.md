---
title: "PageSetup.BottomMarginInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta la dimensione del margine inferiore in unità di pollici"
type: docs
url: /it/net/aspose.cells/pagesetup/bottommargininch/
---
## PageSetup.BottomMarginInch property

Rappresenta la dimensione del margine inferiore, in unità di pollici.

```csharp
public double BottomMarginInch { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBottomMarginInchDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al PageSetup del primo foglio di lavoro
            PageSetup setup = workbook.Worksheets[0].PageSetup;
            
            // Imposta vari margini in pollici
            setup.HeaderMarginInch = 0.1;
            setup.FooterMarginInch = 0.2;
            setup.TopMarginInch = 0.3;
            setup.BottomMarginInch = 0.4; // Demonstrating BottomMarginInch property
            setup.LeftMarginInch = 0.5;
            setup.RightMarginInch = 0.6;
            
            // Salva la cartella di lavoro
            workbook.Save("PageMarginsDemo.xlsx");
            
            // Mostra conferma
            Console.WriteLine("Workbook saved with bottom margin set to: " + setup.BottomMarginInch + " inches");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


