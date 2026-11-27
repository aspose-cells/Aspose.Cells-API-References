---
title: "ThemeColor.ThemeColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThemeColor konstruktor."
type: docs
url: /sv/net/aspose.cells/themecolor/themecolor/
---
## ThemeColor constructor

```csharp
public ThemeColor(ThemeColorType type, double tint)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | ThemeColorType | Tematypen. |
| nyans | Double | Nyansvärdet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThemeColorMethodCtorWithThemeColorTypeDoubleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Anropa #ctor-metoden med ThemeColorType- och Double-parametrar.
                ThemeColor themeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

                // Applicera temafärgen på en cells stil.
                Style style = workbook.CreateStyle();
                style.ForegroundThemeColor = themeColor;
                style.Pattern = BackgroundType.Solid;
                
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("ThemeColor with Accent1 and 0.5 tint");
                cell.SetStyle(style);

                Console.WriteLine("ThemeColor constructor executed successfully with parameters (ThemeColorType.Accent1, 0.5)");
                Console.WriteLine($"ColorType: {themeColor.ColorType}, Tint: {themeColor.Tint}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ThemeColor constructor: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("ThemeColorCtorDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ThemeColorType](../../themecolortype/)
* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


