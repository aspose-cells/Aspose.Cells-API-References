---
title: "Workbook.GetMatchingColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Trova il colore più corrispondente nella palette corrente"
type: docs
url: /it/net/aspose.cells/workbook/getmatchingcolor/
---
## Workbook.GetMatchingColor method

Trova il colore più corrispondente nella tavolozza corrente.

```csharp
public Color GetMatchingColor(Color rawColor)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rawColor | Color | Colore grezzo. |

### Valore di ritorno

Colore più corrispondente.

### Osservazioni

Ci sono solo 56 colori nella palette di colori di Excel 97-2003. Se il colore non è nella palette, verrà impostato il colore più simile.

### Esempi

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
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Verifica se il colore esiste nella palette
            Console.WriteLine("Is Red in palette: " + workbook.IsColorInPalette(Color.Red));
            Color testColor = Color.FromArgb(255, 123, 123, 123);
            Console.WriteLine("Is custom color in palette: " + workbook.IsColorInPalette(testColor));

            // Ottieni il colore corrispondente dalla tavolozza
            Color matchedColor = workbook.GetMatchingColor(testColor);
            Console.WriteLine($"Original color: R={testColor.R}, G={testColor.G}, B={testColor.B}");
            Console.WriteLine($"Matched color: R={matchedColor.R}, G={matchedColor.G}, B={matchedColor.B}");

            // Crea un tema personalizzato
            Color[] themeColors = new Color[12];
            for (int i = 0; i < themeColors.Length; i++)
            {
                themeColors[i] = Color.FromArgb(255, 128 + i, 128 + i, 128 + i);
            }
            workbook.CustomTheme("CustomTheme", themeColors);

            // Ottieni il colore del tema
            Color themeColor = workbook.GetThemeColor(ThemeColorType.FollowedHyperlink);
            Console.WriteLine($"Theme color: R={themeColor.R}, G={themeColor.G}, B={themeColor.B}");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


