---
title: "Workbook.GetMatchingColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Hitta bästa matchande Color i aktuell palett"
type: docs
url: /sv/net/aspose.cells/workbook/getmatchingcolor/
---
## Workbook.GetMatchingColor method

Hitta bäst matchande färg i aktuell palett.

```csharp
public Color GetMatchingColor(Color rawColor)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rawColor | Färg | Rå färg. |

### Returvärde

Bästa matchande färg.

### Anmärkningar

Det finns bara 56 färger i färgpaletten i Excel 97-2003. Om färgen inte finns i paletten kommer en liknande färg att sättas.

### Exempel

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
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kontrollera om färgen finns i paletten
            Console.WriteLine("Is Red in palette: " + workbook.IsColorInPalette(Color.Red));
            Color testColor = Color.FromArgb(255, 123, 123, 123);
            Console.WriteLine("Is custom color in palette: " + workbook.IsColorInPalette(testColor));

            // Hämta matchande färg från paletten
            Color matchedColor = workbook.GetMatchingColor(testColor);
            Console.WriteLine($"Original color: R={testColor.R}, G={testColor.G}, B={testColor.B}");
            Console.WriteLine($"Matched color: R={matchedColor.R}, G={matchedColor.G}, B={matchedColor.B}");

            // Skapa ett anpassat tema
            Color[] themeColors = new Color[12];
            for (int i = 0; i < themeColors.Length; i++)
            {
                themeColors[i] = Color.FromArgb(255, 128 + i, 128 + i, 128 + i);
            }
            workbook.CustomTheme("CustomTheme", themeColors);

            // Hämta temafärg
            Color themeColor = workbook.GetThemeColor(ThemeColorType.FollowedHyperlink);
            Console.WriteLine($"Theme color: R={themeColor.R}, G={themeColor.G}, B={themeColor.B}");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


