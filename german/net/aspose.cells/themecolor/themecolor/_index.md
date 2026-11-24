---
title: "ThemeColor.ThemeColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThemeColor Konstruktor."
type: docs
url: /de/net/aspose.cells/themecolor/themecolor/
---
## ThemeColor constructor

```csharp
public ThemeColor(ThemeColorType type, double tint)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | ThemeColorType | Der Typ des Themas. |
| Farbton | Double | Der Farbtonwert. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThemeColorMethodCtorWithThemeColorTypeDoubleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Rufen Sie die #ctor-Methode mit den Parametern ThemeColorType und Double auf
                ThemeColor themeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

                // Wenden Sie die Themenfarbe auf den Stil einer Zelle an
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
            
            // Ergebnis speichern
            workbook.Save("ThemeColorCtorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ThemeColorType](../../themecolortype/)
* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


