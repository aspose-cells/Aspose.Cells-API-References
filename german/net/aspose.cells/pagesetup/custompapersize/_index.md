---
title: "PageSetup.CustomPaperSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup‑Methode. Legt die benutzerdefinierte Papiergröße in Zoll fest."
type: docs
url: /de/net/aspose.cells/pagesetup/custompapersize/
---
## PageSetup.CustomPaperSize method

Legt die benutzerdefinierte Papiergröße in Zoll fest.

```csharp
public void CustomPaperSize(double width, double height)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Breite | Double | Die Breite des Papiers. |
| Höhe | Double | Die Höhe des Papiers. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodCustomPaperSizeWithDoubleDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setze benutzerdefinierte Papiergröße (Breite: 1,5 Zoll, Höhe: 1,5 Zoll).
            worksheet.PageSetup.CustomPaperSize(1.5, 1.5);
            
            // Speichere die Arbeitsmappe, um die Wirkung zu demonstrieren
            workbook.Save("CustomPaperSizeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


