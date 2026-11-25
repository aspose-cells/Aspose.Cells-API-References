---
title: "PageSetup.LeftMargin"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta la dimensione del margine sinistro in unità di centimetri"
type: docs
url: /it/net/aspose.cells/pagesetup/leftmargin/
---
## PageSetup.LeftMargin property

Rappresenta la dimensione del margine sinistro, in unità di centimetri.

```csharp
public double LeftMargin { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyLeftMarginDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Imposta alcuni dati di esempio
            sheet.Cells["A1"].PutValue("Left Margin Demonstration");
            sheet.Cells["A2"].PutValue("This shows how to set page margins");

            // Imposta il margine sinistro (in pollici)
            sheet.PageSetup.LeftMargin = 1.5;

            // Stampa il valore del margine sinistro nella console
            Console.WriteLine("Left Margin set to: " + sheet.PageSetup.LeftMargin + " inches");

            // Salva in PDF per dimostrare il margine
            string outputPath = "LeftMarginDemo.pdf";
            workbook.Save(outputPath, SaveFormat.Pdf);

            Console.WriteLine("File saved with left margin: " + outputPath);
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


