---
title: "PageSetup.TopMargin"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta la dimensione del margine superiore in unità di centimetri"
type: docs
url: /it/net/aspose.cells/pagesetup/topmargin/
---
## PageSetup.TopMargin property

Rappresenta la dimensione del margine superiore, in centimetri.

```csharp
public double TopMargin { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyTopMarginDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            sheet.Cells["A1"].PutValue("Top Margin Demonstration");
            sheet.Cells["A2"].PutValue("This shows the effect of TopMargin property");

            // Imposta le proprietà di configurazione della pagina
            PageSetup pageSetup = sheet.PageSetup;
            pageSetup.TopMargin = 2.0; // 2 inches top margin
            pageSetup.LeftMargin = 0.5;
            pageSetup.RightMargin = 0.5;
            pageSetup.BottomMargin = 1.0;

            // Salva in PDF per dimostrare i margini
            string outputPath = "TopMarginDemo.pdf";
            workbook.Save(outputPath, SaveFormat.Pdf);

            Console.WriteLine("Document with top margin of 2 inches saved to: " + outputPath);
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


