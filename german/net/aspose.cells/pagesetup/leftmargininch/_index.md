---
title: "PageSetup.LeftMarginInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt die Größe des linken Randes in Zoll an"
type: docs
url: /de/net/aspose.cells/pagesetup/leftmargininch/
---
## PageSetup.LeftMarginInch property

Stellt die Größe des linken Randes in Zoll dar.

```csharp
public double LeftMarginInch { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyLeftMarginInchDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Zugriff auf PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Linken Rand in Zoll festlegen (0,39 Zoll = ~1 cm)
            pageSetup.LeftMarginInch = 0.39;

            // Fügen Sie einige Daten hinzu, um den Rand zu demonstrieren
            worksheet.Cells["A1"].PutValue("Left Margin Demonstration");
            worksheet.Cells["A2"].PutValue("Left margin set to 0.39 inches");

            // Speichere die Arbeitsmappe
            workbook.Save("LeftMarginInchDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


