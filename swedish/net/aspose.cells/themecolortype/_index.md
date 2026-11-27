---
title: "Enum ThemeColorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ThemeColorType enum. Enumererar temafärgstyporna"
type: docs
url: /sv/net/aspose.cells/themecolortype/
---
## ThemeColorType enumeration

Enumererar temafärgtyper.

```csharp
public enum ThemeColorType
```

### Värden

| Namn | Värde | Beskrivning |
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
| StyleColor | `12` | Inner används. En färg som används i temadefinitioner vilket betyder att använda stilens färg. |

### Exempel

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
            
            // Få åtkomst till cell A1 och hämta dess stil
            Style style = cells["A1"].GetStyle();
            
            // Ställ in solid mönster med röd förgrundsfärg
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;
            Console.WriteLine("Foreground ARGB Color: " + style.ForegroundArgbColor);
            
            // Ställ in gray12-mönster med blå förgrund och gul bakgrund
            style.Pattern = BackgroundType.Gray12;
            style.ForegroundColor = Color.Blue;
            style.BackgroundColor = Color.Yellow;
            Console.WriteLine("Foreground ARGB Color: " + style.ForegroundArgbColor);
            Console.WriteLine("Background ARGB Color: " + style.BackgroundArgbColor);
            
            // Ställ in temafärger
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

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


