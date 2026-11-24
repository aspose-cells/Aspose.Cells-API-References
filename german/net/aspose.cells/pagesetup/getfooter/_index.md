---
title: "PageSetup.GetFooter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Methode. Holt ein Skript, das die Fußzeile einer Excel‑Datei formatiert."
type: docs
url: /de/net/aspose.cells/pagesetup/getfooter/
---
## PageSetup.GetFooter method

Ruft ein Skript ab, das die Fußzeile einer Excel-Datei formatiert.

```csharp
public string GetFooter(int section)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | Int32 | 0: Linker Abschnitt, 1: Mittlerer Abschnitt, 2: Rechter Abschnitt. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetFooterWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Verschiedene Fußzeilenabschnitte festlegen
            worksheet.PageSetup.SetFooter(1, "odd");
            worksheet.PageSetup.SetFirstPageFooter(1, "first");
            worksheet.PageSetup.SetEvenFooter(1, "even");

            // Abrufen und Anzeigen der Fußzeilenabschnitte
            Console.WriteLine("First Page Footer: " + worksheet.PageSetup.GetFirstPageFooter(1));
            Console.WriteLine("Even Page Footer: " + worksheet.PageSetup.GetEvenFooter(1));
            Console.WriteLine("Odd Page Footer: " + worksheet.PageSetup.GetFooter(1));
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


