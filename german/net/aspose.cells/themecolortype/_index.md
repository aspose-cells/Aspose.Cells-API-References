---
title: "Enum ThemeColorType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ThemeColorType enum. Enumeriert die Theme-Farbtypen"
type: docs
url: /de/net/aspose.cells/themecolortype/
---
## ThemeColorType enumeration

Enumeriert die Themenfarbtypen.

```csharp
public enum ThemeColorType
```

### Werte

| Name | Wert | Beschreibung |
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
| StyleColor | `12` | Inner verwendet. Eine Farbe, die in Theme-Definitionen verwendet wird und bedeutet, die Farbe des Stils zu nutzen. |

### Beispiele

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
            
            // Greifen Sie auf die Zelle A1 zu und erhalten Sie deren Stil
            Style style = cells["A1"].GetStyle();
            
            // Setzen Sie ein solides Muster mit roter Vordergrundfarbe
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;
            Console.WriteLine("Foreground ARGB Color: " + style.ForegroundArgbColor);
            
            // Setzen Sie das gray12-Muster mit blauem Vordergrund und gelbem Hintergrund
            style.Pattern = BackgroundType.Gray12;
            style.ForegroundColor = Color.Blue;
            style.BackgroundColor = Color.Yellow;
            Console.WriteLine("Foreground ARGB Color: " + style.ForegroundArgbColor);
            Console.WriteLine("Background ARGB Color: " + style.BackgroundArgbColor);
            
            // Setzen Sie Theme-Farben
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

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


