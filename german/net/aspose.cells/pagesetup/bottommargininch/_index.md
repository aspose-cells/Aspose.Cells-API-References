---
title: "PageSetup.BottomMarginInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt die Größe des unteren Randes in Zoll an."
type: docs
url: /de/net/aspose.cells/pagesetup/bottommargininch/
---
## PageSetup.BottomMarginInch property

Gibt die Größe des unteren Randes in Zoll an.

```csharp
public double BottomMarginInch { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBottomMarginInchDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf das PageSetup des ersten Arbeitsblatts zu.
            PageSetup setup = workbook.Worksheets[0].PageSetup;
            
            // Legen Sie verschiedene Ränder in Zoll fest.
            setup.HeaderMarginInch = 0.1;
            setup.FooterMarginInch = 0.2;
            setup.TopMarginInch = 0.3;
            setup.BottomMarginInch = 0.4; // Demonstrating BottomMarginInch property
            setup.LeftMarginInch = 0.5;
            setup.RightMarginInch = 0.6;
            
            // Speichere die Arbeitsmappe
            workbook.Save("PageMarginsDemo.xlsx");
            
            // Bestätigung anzeigen
            Console.WriteLine("Workbook saved with bottom margin set to: " + setup.BottomMarginInch + " inches");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


