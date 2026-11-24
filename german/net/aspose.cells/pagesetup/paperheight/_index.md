---
title: "PageSetup.PaperHeight"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt die Höhe des Papiers in Zoll zurück, wobei die Seitenausrichtung berücksichtigt wird"
type: docs
url: /de/net/aspose.cells/pagesetup/paperheight/
---
## PageSetup.PaperHeight property

Liest die Höhe des Papiers in Zoll, unter Berücksichtigung der Seitenorientierung.

```csharp
public double PaperHeight { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperHeightDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige Daten in einer Zelle festlegen
            worksheet.Cells["A1"].PutValue("Paper Height Demo");
            
            // Das PageSetup-Objekt abrufen
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Standard-Papierhöhe (in Zoll) anzeigen
            Console.WriteLine("Default Paper Height: " + pageSetup.PaperHeight);
            
            // PaperHeight ist schreibgeschützt, daher demonstrieren wir das Abrufen verschiedener Papiergrößen
            // indem der Papiertyp auf Letter (8,5 × 11 Zoll) geändert wird
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            
            // Die Änderung überprüfen
            Console.WriteLine("Modified Paper Height (Letter size): " + pageSetup.PaperHeight);
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


