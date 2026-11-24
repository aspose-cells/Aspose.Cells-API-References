---
title: "PageSetup.FooterMargin"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt den Abstand vom unteren Rand der Seite bis zur Fußzeile in Zentimetern an."
type: docs
url: /de/net/aspose.cells/pagesetup/footermargin/
---
## PageSetup.FooterMargin property

Gibt den Abstand vom unteren Rand der Seite bis zur Fußzeile in Zentimetern an.

```csharp
public double FooterMargin { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFooterMarginDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Zugriff auf PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Fußzeilenrand in Zentimetern festlegen
            pageSetup.FooterMargin = 1.5;

            // Fügen Sie etwas Inhalt hinzu, um die Wirkung zu sehen
            worksheet.Cells["A1"].PutValue("Footer Margin Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates setting footer margin to 1.5 cm");

            // Fußzeilentext festlegen, um den Rand sichtbar zu machen
            pageSetup.SetFooter(0, "&A - Footer text to demonstrate margin");

            // Speichere die Arbeitsmappe
            workbook.Save("FooterMarginDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


