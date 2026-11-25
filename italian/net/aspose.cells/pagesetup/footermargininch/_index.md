---
title: "PageSetup.FooterMarginInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta la distanza dal fondo della pagina al piè di pagina in unità di pollici"
type: docs
url: /it/net/aspose.cells/pagesetup/footermargininch/
---
## PageSetup.FooterMarginInch property

Rappresenta la distanza dal bordo inferiore della pagina al piè di pagina, in unità di pollici.

```csharp
public double FooterMarginInch { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFooterMarginInchDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e al suo PageSetup
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Imposta il margine del piè di pagina in pollici
            pageSetup.FooterMarginInch = 0.5;
            
            // Imposta altri margini per dimostrazione
            pageSetup.HeaderMarginInch = 0.3;
            pageSetup.TopMarginInch = 1.0;
            pageSetup.BottomMarginInch = 1.0;
            pageSetup.LeftMarginInch = 0.75;
            pageSetup.RightMarginInch = 0.75;
            
            // Salva la cartella di lavoro
            workbook.Save("PageSetupMargins.xlsx");
            
            // Stampa conferma
            Console.WriteLine("Footer margin set to: " + pageSetup.FooterMarginInch + " inches");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


