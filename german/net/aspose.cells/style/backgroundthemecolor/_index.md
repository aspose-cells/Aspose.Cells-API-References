---
title: "Style.BackgroundThemeColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt die Hintergrund-Theme-Farbe zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells/style/backgroundthemecolor/
---
## Style.BackgroundThemeColor property

Liest und setzt die Hintergrund‑Themenfarbe.

```csharp
public ThemeColor BackgroundThemeColor { get; set; }
```

### Hinweise

Wenn die Hintergrundfarbe keine Theme-Farbe ist, wird NULL zurückgegeben.

### Beispiele

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

            // Erstelle einen Stil und setze die Hintergrund-Theme-Farbe
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            
            ThemeColor themeColor = new ThemeColor(ThemeColorType.Accent2, 0.5);
            style.BackgroundThemeColor = themeColor;

            // Wende den Stil auf eine Zelle an
            cells["A1"].SetStyle(style);

            // Überprüfe die Hintergrund-Theme-Farbe
            ThemeColor retrievedColor = cells["A1"].GetStyle().BackgroundThemeColor;
            Console.WriteLine("Background Theme Color Type: " + retrievedColor.ColorType);
            Console.WriteLine("Background Theme Color Tint: " + retrievedColor.Tint);
        }
    }
}
```

### Siehe auch

* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


