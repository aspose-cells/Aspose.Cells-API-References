---
title: "PageSetup.TopMargin"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt die Größe des oberen Randes in Zentimetern an."
type: docs
url: /de/net/aspose.cells/pagesetup/topmargin/
---
## PageSetup.TopMargin property

Stellt die Größe des oberen Randes in Zentimetern dar.

```csharp
public double TopMargin { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Top Margin Demonstration");
            sheet.Cells["A2"].PutValue("This shows the effect of TopMargin property");

            // Seitenlayout-Eigenschaften festlegen
            PageSetup pageSetup = sheet.PageSetup;
            pageSetup.TopMargin = 2.0; // 2 inches top margin
            pageSetup.LeftMargin = 0.5;
            pageSetup.RightMargin = 0.5;
            pageSetup.BottomMargin = 1.0;

            // Als PDF speichern, um die Ränder zu demonstrieren
            string outputPath = "TopMarginDemo.pdf";
            workbook.Save(outputPath, SaveFormat.Pdf);

            Console.WriteLine("Document with top margin of 2 inches saved to: " + outputPath);
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


