---
title: "PageSetup.HeaderMargin"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta la distanza dalla parte superiore della pagina all'intestazione in unità di centimetri"
type: docs
url: /it/net/aspose.cells/pagesetup/headermargin/
---
## PageSetup.HeaderMargin property

Rappresenta la distanza dal bordo superiore della pagina all'intestazione, in unità di centimetri.

```csharp
public double HeaderMargin { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyHeaderMarginDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi a PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Imposta il margine dell'intestazione in centimetri
            pageSetup.HeaderMargin = 1.5;

            // Verifica che il margine dell'intestazione sia stato impostato
            Console.WriteLine("Header Margin: " + pageSetup.HeaderMargin + " cm");

            // Salva la cartella di lavoro
            workbook.Save("HeaderMarginDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


