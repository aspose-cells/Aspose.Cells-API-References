---
title: "Enum ThemeColorType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.ThemeColorType enum. Elenca i tipi di colore del tema"
type: docs
url: /it/net/aspose.cells/themecolortype/
---
## ThemeColorType enumeration

Enumera i tipi di colore del tema.

```csharp
public enum ThemeColorType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Background1 | `0` |  |
| Text1 | `1` |  |
| Background2 | `2` |  |
| Text2 | `3` |  |
| Accent1 | `4` |  |
| Accent2 | `5` |  |
| Accent3 | `6` |  |
| Accent4 | `7` |  |
| Accent5 | `8` |  |
| Accent6 | `9` |  |
| Hyperlink | `10` |  |
| FollowedHyperlink | `11` |  |
| StyleColor | `12` | Inner usato. Un colore usato nelle definizioni del tema che indica di utilizzare il colore dello stile. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsClassThemeColorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Accedi alla cella A1 e ottieni il suo stile
            Style style = cells["A1"].GetStyle();
            
            // Imposta il modello solido con colore di primo piano rosso
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;
            Console.WriteLine("Foreground ARGB Color: " + style.ForegroundArgbColor);
            
            // Imposta il modello gray12 con primo piano blu e sfondo giallo
            style.Pattern = BackgroundType.Gray12;
            style.ForegroundColor = Color.Blue;
            style.BackgroundColor = Color.Yellow;
            Console.WriteLine("Foreground ARGB Color: " + style.ForegroundArgbColor);
            Console.WriteLine("Background ARGB Color: " + style.BackgroundArgbColor);
            
            // Imposta i colori del tema
            ThemeColor foregroundTheme = new ThemeColor(ThemeColorType.Accent6, 0.5);
            ThemeColor backgroundTheme = new ThemeColor(ThemeColorType.Accent2, 0.5);
            style.ForegroundThemeColor = foregroundTheme;
            style.BackgroundThemeColor = backgroundTheme;
            
            Console.WriteLine("Foreground Theme Color Type: " + style.ForegroundThemeColor.ColorType);
            Console.WriteLine("Background Theme Color Type: " + style.BackgroundThemeColor.ColorType);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


