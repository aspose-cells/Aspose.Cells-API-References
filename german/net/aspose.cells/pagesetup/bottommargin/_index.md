---
title: "PageSetup.BottomMargin"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt die Größe des unteren Randes in Zentimetern an"
type: docs
url: /de/net/aspose.cells/pagesetup/bottommargin/
---
## PageSetup.BottomMargin property

Gibt die Größe des unteren Randes in Zentimetern an.

```csharp
public double BottomMargin { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten festlegen
            worksheet.Cells["A1"].PutValue("Sample Text for Margin Demonstration");
            
            // Konfiguriere die Seiteneinrichtung mit BottomMargin
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.BottomMargin = 0.5; // 0.5 inch bottom margin
            pageSetup.TopMargin = 1.0;    // 1 inch top margin
            pageSetup.LeftMargin = 0.75;  // 0.75 inch left margin
            pageSetup.RightMargin = 0.75; // 0.75 inch right margin

            // Als PDF speichern, um die Ränder zu demonstrieren
            workbook.Save("PageMarginsDemo.pdf", SaveFormat.Pdf);

            Console.WriteLine("Document with bottom margin of 0.5 inches created successfully.");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


