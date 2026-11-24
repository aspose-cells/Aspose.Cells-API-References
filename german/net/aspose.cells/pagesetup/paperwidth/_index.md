---
title: "PageSetup.PaperWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup‑Eigenschaft. Gibt die Breite des Papiers in Zoll an, unter Berücksichtigung der Seitenausrichtung."
type: docs
url: /de/net/aspose.cells/pagesetup/paperwidth/
---
## PageSetup.PaperWidth property

Liest die Breite des Papiers in Zoll, unter Berücksichtigung der Seitenorientierung.

```csharp
public double PaperWidth { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperWidthDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten festlegen
            worksheet.Cells["A1"].PutValue("Sample Page Setup Demo");
            
            // Zugriff auf die Seiteneinrichtung des Arbeitsblatts
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Demonstriere die PaperWidth‑Eigenschaft (schreibgeschützt).
            Console.WriteLine("Paper Width: " + pageSetup.PaperWidth);
            
            // Um die Papiergröße zu ändern, verwende stattdessen die PaperSize‑Eigenschaft.
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            Console.WriteLine("New Paper Width: " + pageSetup.PaperWidth);
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


