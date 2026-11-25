---
title: "PageSetup.RightMarginInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta la dimensione del margine destro nell'unità di pollici"
type: docs
url: /it/net/aspose.cells/pagesetup/rightmargininch/
---
## PageSetup.RightMarginInch property

Rappresenta la dimensione del margine destro, in pollici.

```csharp
public double RightMarginInch { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyRightMarginInchDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi a PageSetup e imposta RightMarginInch
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.RightMarginInch = 0.75; // Set right margin to 0.75 inches

            // Aggiungi alcuni dati di esempio per vedere l'effetto
            worksheet.Cells["A1"].PutValue("Right Margin Demo");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["B" + i].PutValue("Sample Data " + i);
            }

            // Salva la cartella di lavoro
            workbook.Save("RightMarginInchDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


