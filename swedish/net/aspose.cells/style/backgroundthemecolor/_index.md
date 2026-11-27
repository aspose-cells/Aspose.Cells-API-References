---
title: "Style.BackgroundThemeColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style‑egenskap. Hämtar och anger bakgrundens temafärg"
type: docs
url: /sv/net/aspose.cells/style/backgroundthemecolor/
---
## Style.BackgroundThemeColor property

Hämtar och anger bakgrundens temafärg.

```csharp
public ThemeColor BackgroundThemeColor { get; set; }
```

### Anmärkningar

Om bakgrundsfärgen inte är en temafärg returneras NULL.

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyBackgroundThemeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa en stil och ange bakgrundstemat färg
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            
            ThemeColor themeColor = new ThemeColor(ThemeColorType.Accent2, 0.5);
            style.BackgroundThemeColor = themeColor;

            // Tillämpa stilen på en cell
            cells["A1"].SetStyle(style);

            // Verifiera bakgrundstemat färg
            ThemeColor retrievedColor = cells["A1"].GetStyle().BackgroundThemeColor;
            Console.WriteLine("Background Theme Color Type: " + retrievedColor.ColorType);
            Console.WriteLine("Background Theme Color Tint: " + retrievedColor.Tint);
        }
    }
}
```

### Se även

* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


