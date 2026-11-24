---
title: "CellsColor.ThemeColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsColor‑Eigenschaft. Gibt die Themenfarbe zurück. Gilt nur für den Typ Themenfarbe."
type: docs
url: /de/net/aspose.cells/cellscolor/themecolor/
---
## CellsColor.ThemeColor property

Liest die Themenfarbe. Gilt nur für den Typ Themenfarbe.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsColorPropertyThemeColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Erstellen Sie eine CellsColor‑Instanz
                CellsColor cellsColor = workbook.CreateCellsColor();

                // Setze eine Themenfarbe.
                cellsColor.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

                // Zeige die ThemeColor‑Eigenschaften an.
                Console.WriteLine("ThemeColor Type: " + cellsColor.ThemeColor.ColorType);
                Console.WriteLine("ThemeColor Tint: " + cellsColor.ThemeColor.Tint);

                // Wende die Farbe auf eine Zelle an.
                Style style = workbook.CreateStyle();
                style.ForegroundColor = cellsColor.Color;
                style.Pattern = BackgroundType.Solid;

                worksheet.Cells["A1"].PutValue("Theme Color Example");
                worksheet.Cells["A1"].SetStyle(style);

                // Speichere die Arbeitsmappe
                workbook.Save("ThemeColorDemo.xlsx");
                Console.WriteLine("ThemeColor has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [ThemeColor](../../themecolor/)
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


