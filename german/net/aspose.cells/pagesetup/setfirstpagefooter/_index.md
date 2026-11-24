---
title: "PageSetup.SetFirstPageFooter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Methode. Legt ein Skript fest, das die Fußzeile der ersten Seite einer Excel-Datei formatiert"
type: docs
url: /de/net/aspose.cells/pagesetup/setfirstpagefooter/
---
## PageSetup.SetFirstPageFooter method

Legt ein Skript fest, das die Fußzeile der ersten Seite einer Excel-Datei formatiert.

```csharp
public void SetFirstPageFooter(int section, string footerScript)
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
    public class PageSetupMethodSetFirstPageFooterWithInt32StringDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Das PageSetup-Objekt abrufen
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Unterschiedliche Kopf‑/Fußzeilen für die erste Seite festlegen
            pageSetup.IsHFDiffFirst = true;
            
            // Fußzeile der ersten Seite mit Abschnittsindex und Text festlegen
            pageSetup.SetFirstPageFooter(0, "First Page Footer Text");
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            Console.WriteLine("First page footer set successfully.");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


