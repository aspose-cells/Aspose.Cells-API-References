---
title: "PageSetup.HeaderMargin"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt den Abstand vom oberen Rand der Seite bis zur Kopfzeile in Zentimetern an."
type: docs
url: /de/net/aspose.cells/pagesetup/headermargin/
---
## PageSetup.HeaderMargin property

Gibt den Abstand vom oberen Rand der Seite bis zur Kopfzeile in Zentimetern an.

```csharp
public double HeaderMargin { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyHeaderMarginDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Zugriff auf PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Kopfzeilenrand in Zentimetern festlegen
            pageSetup.HeaderMargin = 1.5;

            // Überprüfen Sie, ob der Kopfzeilenrand gesetzt wurde
            Console.WriteLine("Header Margin: " + pageSetup.HeaderMargin + " cm");

            // Speichere die Arbeitsmappe
            workbook.Save("HeaderMarginDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


