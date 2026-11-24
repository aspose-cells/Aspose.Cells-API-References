---
title: "PageSetup.GetFirstPageHeader"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup‑Methode. Gibt ein Skript zurück, das die erste Seitenkopfzeile einer Excel‑Datei formatiert"
type: docs
url: /de/net/aspose.cells/pagesetup/getfirstpageheader/
---
## PageSetup.GetFirstPageHeader method

Ruft ein Skript ab, das die Kopfzeile der ersten Seite einer Excel-Datei formatiert.

```csharp
public string GetFirstPageHeader(int section)
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
    public class PageSetupMethodGetFirstPageHeaderWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zugriff auf PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Unterschiedliche Kopf‑/Fußzeile für die erste Seite aktivieren
            pageSetup.IsHFDiffFirst = true;
            
            // Abschnitte der ersten Seitenkopfzeile festlegen
            pageSetup.SetFirstPageHeader(0, "&LFirst Page Left Header");
            pageSetup.SetFirstPageHeader(1, "&CFirst Page Center Header");
            pageSetup.SetFirstPageHeader(2, "&RFirst Page Right Header");
            
            // Erhalte und zeige die Abschnitte der ersten Seitenkopfzeile an
            Console.WriteLine("First Page Header Sections:");
            Console.WriteLine("Left: " + pageSetup.GetFirstPageHeader(0));
            Console.WriteLine("Center: " + pageSetup.GetFirstPageHeader(1));
            Console.WriteLine("Right: " + pageSetup.GetFirstPageHeader(2));
            
            // Speichere die Arbeitsmappe
            workbook.Save("PageSetupFirstPageHeaderDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


