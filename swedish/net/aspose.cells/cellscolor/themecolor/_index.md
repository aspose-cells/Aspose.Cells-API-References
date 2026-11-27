---
title: "CellsColor.ThemeColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsColor property. Hämtar temafärgen. Gäller endast för temafärgstyp"
type: docs
url: /sv/net/aspose.cells/cellscolor/themecolor/
---
## CellsColor.ThemeColor property

Hämtar temafärgen. Gäller endast för temafärgstyp.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Skapa en CellsColor-instans
                CellsColor cellsColor = workbook.CreateCellsColor();

                // Ställ in en temafärg
                cellsColor.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

                // Visa ThemeColor-egenskaperna
                Console.WriteLine("ThemeColor Type: " + cellsColor.ThemeColor.ColorType);
                Console.WriteLine("ThemeColor Tint: " + cellsColor.ThemeColor.Tint);

                // Applicera färgen på en cell
                Style style = workbook.CreateStyle();
                style.ForegroundColor = cellsColor.Color;
                style.Pattern = BackgroundType.Solid;

                worksheet.Cells["A1"].PutValue("Theme Color Example");
                worksheet.Cells["A1"].SetStyle(style);

                // Spara arbetsboken
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

### Se även

* class [ThemeColor](../../themecolor/)
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


