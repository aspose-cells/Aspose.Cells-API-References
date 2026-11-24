---
title: "PageSetup.FooterMarginInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt den Abstand vom unteren Rand der Seite bis zur Fußzeile in Zoll an"
type: docs
url: /de/net/aspose.cells/pagesetup/footermargininch/
---
## PageSetup.FooterMarginInch property

Gibt den Abstand vom unteren Rand der Seite bis zur Fußzeile in Zoll an.

```csharp
public double FooterMarginInch { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFooterMarginInchDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Erstes Arbeitsblatt und dessen PageSetup aufrufen
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Fußzeilenrand in Zoll festlegen
            pageSetup.FooterMarginInch = 0.5;
            
            // Weitere Ränder zur Demonstration festlegen
            pageSetup.HeaderMarginInch = 0.3;
            pageSetup.TopMarginInch = 1.0;
            pageSetup.BottomMarginInch = 1.0;
            pageSetup.LeftMarginInch = 0.75;
            pageSetup.RightMarginInch = 0.75;
            
            // Speichere die Arbeitsmappe
            workbook.Save("PageSetupMargins.xlsx");
            
            // Druckbestätigung
            Console.WriteLine("Footer margin set to: " + pageSetup.FooterMarginInch + " inches");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


