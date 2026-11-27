---
title: "Workbook.IsColorInPalette"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Kontrollerar om en färg finns i paletten för kalkylbladet"
type: docs
url: /sv/net/aspose.cells/workbook/iscolorinpalette/
---
## Workbook.IsColorInPalette method

Kontrollerar om en färg finns i paletten för kalkylbladet.

```csharp
public bool IsColorInPalette(Color color)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| färg | Färg | Färgsstruktur. |

### Returvärde

Returnerar true om denna färg finns i paletten. Annars returneras false

### Exempel

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
            
            // Kontrollera om standardfärgen finns i paletten
            bool isRedInPalette = workbook.IsColorInPalette(Color.Red);
            Console.WriteLine("Is Red in palette: " + isRedInPalette);
            
            // Kontrollera om anpassad färg finns i paletten
            Color customColor = Color.FromArgb(255, 123, 123, 123);
            bool isCustomInPalette = workbook.IsColorInPalette(customColor);
            Console.WriteLine("Is custom color in palette: " + isCustomInPalette);
            
            // Hämta matchande färg från paletten
            Color matchedColor = workbook.GetMatchingColor(customColor);
            Console.WriteLine("Matched color R value: " + matchedColor.R);
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


