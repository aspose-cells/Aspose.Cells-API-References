---
title: "PageSetup.TopMarginInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta la dimensione del margine superiore nell'unità di pollici"
type: docs
url: /it/net/aspose.cells/pagesetup/topmargininch/
---
## PageSetup.TopMarginInch property

Rappresenta la dimensione del margine superiore, in pollici.

```csharp
public double TopMarginInch { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyTopMarginInchDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Imposta il margine superiore a 1,5 pollici
            sheet.PageSetup.TopMarginInch = 1.5;

            // Ottieni e stampa il valore del margine superiore
            Console.WriteLine("Top Margin (inches): " + sheet.PageSetup.TopMarginInch);

            // Salva la cartella di lavoro
            workbook.Save("PageSetup_TopMarginInch_Example.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


