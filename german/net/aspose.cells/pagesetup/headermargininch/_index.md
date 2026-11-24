---
title: "PageSetup.HeaderMarginInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt den Abstand vom oberen Rand der Seite bis zum Header in Zoll an"
type: docs
url: /de/net/aspose.cells/pagesetup/headermargininch/
---
## PageSetup.HeaderMarginInch property

Gibt den Abstand vom oberen Rand der Seite bis zur Kopfzeile in Zoll an.

```csharp
public double HeaderMarginInch { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyHeaderMarginInchDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf das erste Arbeitsblatt und dessen PageSetup zu
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Setzen Sie den Header-Abstand in Zoll
            pageSetup.HeaderMarginInch = 0.5;
            
            // Weitere Ränder zur Demonstration festlegen
            pageSetup.FooterMarginInch = 0.25;
            pageSetup.TopMarginInch = 1.0;
            pageSetup.BottomMarginInch = 1.0;
            pageSetup.LeftMarginInch = 0.75;
            pageSetup.RightMarginInch = 0.75;

            // Speichere die Arbeitsmappe
            workbook.Save("PageSetupMargins.xlsx");

            // Zeigen Sie den Wert des Header-Abstands an
            Console.WriteLine("Header Margin (inches): " + pageSetup.HeaderMarginInch);
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


