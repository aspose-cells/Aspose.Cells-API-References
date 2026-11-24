---
title: "PageSetup.TopMarginInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt die Größe des oberen Randes in Zoll an"
type: docs
url: /de/net/aspose.cells/pagesetup/topmargininch/
---
## PageSetup.TopMarginInch property

Stellt die Größe des oberen Randes in Zoll dar.

```csharp
public double TopMarginInch { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyTopMarginInchDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Setze den oberen Rand auf 1,5 Zoll
            sheet.PageSetup.TopMarginInch = 1.5;

            // Lese und gib den Wert des oberen Randes aus
            Console.WriteLine("Top Margin (inches): " + sheet.PageSetup.TopMarginInch);

            // Speichere die Arbeitsmappe
            workbook.Save("PageSetup_TopMarginInch_Example.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


