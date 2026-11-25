---
title: "PageSetup.LeftMarginInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PageSetup proprietà. Rappresenta la dimensione del margine sinistro in unità di pollici"
type: docs
url: /it/net/aspose.cells/pagesetup/leftmargininch/
---
## PageSetup.LeftMarginInch property

Rappresenta la dimensione del margine sinistro, in unità di pollici.

```csharp
public double LeftMarginInch { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyLeftMarginInchDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi a PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Imposta il margine sinistro in pollici (0,39 pollici = ~1 cm)
            pageSetup.LeftMarginInch = 0.39;

            // Aggiungi alcuni dati per dimostrare il margine
            worksheet.Cells["A1"].PutValue("Left Margin Demonstration");
            worksheet.Cells["A2"].PutValue("Left margin set to 0.39 inches");

            // Salva la cartella di lavoro
            workbook.Save("LeftMarginInchDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


