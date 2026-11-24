---
title: "PageSetup.GetEvenFooter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Methode. Ruft ein Skript ab, das die gerade Fußzeile einer Excel-Datei formatiert"
type: docs
url: /de/net/aspose.cells/pagesetup/getevenfooter/
---
## PageSetup.GetEvenFooter method

Ruft ein Skript ab, das die gerade Fußzeile einer Excel-Datei formatiert.

```csharp
public string GetEvenFooter(int section)
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
    public class PageSetupMethodGetEvenFooterWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Aktiviere unterschiedliche Kopf‑/Fußzeilen für ungerade und gerade Seiten
            pageSetup.IsHFDiffOddEven = true;
            
            // Gerade Fußzeile festlegen
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            
            // Gerade Fußzeile abrufen und anzeigen
            string evenFooter = pageSetup.GetEvenFooter(0);
            Console.WriteLine("Even Footer: " + evenFooter);
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


