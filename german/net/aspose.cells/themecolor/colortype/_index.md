---
title: "ThemeColor.ColorType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThemeColor Eigenschaft. Liest und setzt den Thementyp"
type: docs
url: /de/net/aspose.cells/themecolor/colortype/
---
## ThemeColor.ColorType property

Liest und setzt den Thementyp.

```csharp
public ThemeColorType ColorType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThemeColorPropertyColorTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle zwei Themenfarben mit unterschiedlichen Typen
            ThemeColor color1 = new ThemeColor(ThemeColorType.Accent1, 0.5);
            ThemeColor color2 = new ThemeColor(ThemeColorType.Accent2, 0.3);
            
            // Demonstriere die ColorType-Eigenschaft
            Console.WriteLine("Color1 Type: " + color1.ColorType);
            Console.WriteLine("Color2 Type: " + color2.ColorType);
            
            // Wende Themenfarben auf Zellen an
            Style style1 = workbook.CreateStyle();
            style1.ForegroundThemeColor = color1;
            worksheet.Cells["A1"].SetStyle(style1);
            
            Style style2 = workbook.CreateStyle();
            style2.ForegroundThemeColor = color2;
            worksheet.Cells["A2"].SetStyle(style2);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ThemeColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ThemeColorType](../../themecolortype/)
* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


