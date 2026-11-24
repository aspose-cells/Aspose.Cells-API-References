---
title: "PageSetup.SetEvenFooter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Methode. Legt ein Skript fest, das die Fußzeile der geraden Seiten einer Excel‑Datei formatiert. Wirkt nur in Excel 2007, wenn IsHFDiffOddEven true ist."
type: docs
url: /de/net/aspose.cells/pagesetup/setevenfooter/
---
## PageSetup.SetEvenFooter method

Legt ein Skript fest, das die gerade Seitenfußzeile einer Excel-Datei formatiert. Wirkt nur in Excel 2007, wenn IsHFDiffOddEven true ist.

```csharp
public void SetEvenFooter(int section, string footerScript)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | Int32 | 0: Linker Abschnitt, 1: Mittlerer Abschnitt, 2: Rechter Abschnitt. |
| footerScript | String | Fußzeilenformatierungs‑Skript. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetEvenFooterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Unterschiedliche Kopf‑ und Fußzeilen für erste und gerade Seiten aktivieren
            pageSetup.IsHFDiffFirst = true;
            pageSetup.IsHFDiffOddEven = true;

            // Verschiedene Fußzeilentypen festlegen
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            pageSetup.SetFooter(0, "Odd Page Footer");
            pageSetup.SetFirstPageFooter(0, "First Page Footer");

            // Speichere die Arbeitsmappe
            workbook.Save("PageSetup_SetEvenFooter_Example.xlsx");

            Console.WriteLine("Workbook saved with even page footer set successfully.");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


