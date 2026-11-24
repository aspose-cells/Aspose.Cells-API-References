---
title: "Workbook.IsColorInPalette"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Prüft, ob eine Farbe in der Palette der Tabelle enthalten ist"
type: docs
url: /de/net/aspose.cells/workbook/iscolorinpalette/
---
## Workbook.IsColorInPalette method

Prüft, ob eine Farbe in der Palette für das Tabellenblatt vorhanden ist.

```csharp
public bool IsColorInPalette(Color color)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Farbe | Farbe | Color-Struktur. |

### Rückgabewert

Gibt true zurück, wenn diese Farbe in der Palette ist. Andernfalls wird false zurückgegeben

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodIsColorInPaletteWithColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Prüfen, ob Standardfarbe in der Palette vorhanden ist
            bool isRedInPalette = workbook.IsColorInPalette(Color.Red);
            Console.WriteLine("Is Red in palette: " + isRedInPalette);
            
            // Prüfen, ob benutzerdefinierte Farbe in der Palette vorhanden ist
            Color customColor = Color.FromArgb(255, 123, 123, 123);
            bool isCustomInPalette = workbook.IsColorInPalette(customColor);
            Console.WriteLine("Is custom color in palette: " + isCustomInPalette);
            
            // Passende Farbe aus der Palette abrufen
            Color matchedColor = workbook.GetMatchingColor(customColor);
            Console.WriteLine("Matched color R value: " + matchedColor.R);
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


