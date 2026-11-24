---
title: "PageSetup.GetFirstPageFooter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Methode. Gibt ein Skript zurück, das die Fußzeile der ersten Seite einer Excel-Datei formatiert"
type: docs
url: /de/net/aspose.cells/pagesetup/getfirstpagefooter/
---
## PageSetup.GetFirstPageFooter method

Ruft ein Skript ab, das die Fußzeile der ersten Seite einer Excel-Datei formatiert.

```csharp
public string GetFirstPageFooter(int section)
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
    public class PageSetupMethodGetFirstPageFooterWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Setze die Fußzeile der ersten Seite
            worksheet.PageSetup.SetFirstPageFooter(1, "First Page Footer");

            // Lese und drucke die Fußzeile der ersten Seite
            string footer = worksheet.PageSetup.GetFirstPageFooter(1);
            Console.WriteLine("First Page Footer: " + footer);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


