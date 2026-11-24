---
title: "Workbook.GetMatchingColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Findet die am besten passende Farbe in der aktuellen Palette"
type: docs
url: /de/net/aspose.cells/workbook/getmatchingcolor/
---
## Workbook.GetMatchingColor method

Findet die am besten passende Farbe in der aktuellen Palette.

```csharp
public Color GetMatchingColor(Color rawColor)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rawColor | Farbe | Rohfarbe. |

### Rückgabewert

Am besten passende Farbe.

### Hinweise

In der Farbpalette von Excel 97-2003 gibt es nur 56 Farben. Wenn die Farbe nicht in der Palette enthalten ist, wird die ähnliche Farbe gesetzt.

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetMatchingColorWithColorDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Prüfen, ob die Farbe in der Palette vorhanden ist
            Console.WriteLine("Is Red in palette: " + workbook.IsColorInPalette(Color.Red));
            Color testColor = Color.FromArgb(255, 123, 123, 123);
            Console.WriteLine("Is custom color in palette: " + workbook.IsColorInPalette(testColor));

            // Passende Farbe aus der Palette abrufen
            Color matchedColor = workbook.GetMatchingColor(testColor);
            Console.WriteLine($"Original color: R={testColor.R}, G={testColor.G}, B={testColor.B}");
            Console.WriteLine($"Matched color: R={matchedColor.R}, G={matchedColor.G}, B={matchedColor.B}");

            // Ein benutzerdefiniertes Design erstellen
            Color[] themeColors = new Color[12];
            for (int i = 0; i < themeColors.Length; i++)
            {
                themeColors[i] = Color.FromArgb(255, 128 + i, 128 + i, 128 + i);
            }
            workbook.CustomTheme("CustomTheme", themeColors);

            // Designfarbe abrufen
            Color themeColor = workbook.GetThemeColor(ThemeColorType.FollowedHyperlink);
            Console.WriteLine($"Theme color: R={themeColor.R}, G={themeColor.G}, B={themeColor.B}");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


