---
title: "PageSetup.BottomMargin"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PageSetup proprietà. Rappresenta la dimensione del margine inferiore in unità di centimetri"
type: docs
url: /it/net/aspose.cells/pagesetup/bottommargin/
---
## PageSetup.BottomMargin property

Rappresenta la dimensione del margine inferiore, in unità di centimetri.

```csharp
public double BottomMargin { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBottomMarginDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("Sample Text for Margin Demonstration");
            
            // Configura l'impostazione della pagina con BottomMargin
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.BottomMargin = 0.5; // 0.5 inch bottom margin
            pageSetup.TopMargin = 1.0;    // 1 inch top margin
            pageSetup.LeftMargin = 0.75;  // 0.75 inch left margin
            pageSetup.RightMargin = 0.75; // 0.75 inch right margin

            // Salva in PDF per dimostrare i margini
            workbook.Save("PageMarginsDemo.pdf", SaveFormat.Pdf);

            Console.WriteLine("Document with bottom margin of 0.5 inches created successfully.");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


