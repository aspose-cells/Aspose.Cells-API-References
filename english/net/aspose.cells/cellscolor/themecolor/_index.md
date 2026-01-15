---
title: CellsColor.ThemeColor
second_title: Aspose.Cells for .NET API Reference
description: CellsColor property. Gets the theme color. Only applies for theme color type
type: docs
url: /net/aspose.cells/cellscolor/themecolor/
---
## CellsColor.ThemeColor property

Gets the theme color. Only applies for theme color type.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Examples

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
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Create a CellsColor instance
                CellsColor cellsColor = workbook.CreateCellsColor();

                // Set a theme color
                cellsColor.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

                // Display the ThemeColor properties
                Console.WriteLine("ThemeColor Type: " + cellsColor.ThemeColor.ColorType);
                Console.WriteLine("ThemeColor Tint: " + cellsColor.ThemeColor.Tint);

                // Apply the color to a cell
                Style style = workbook.CreateStyle();
                style.ForegroundColor = cellsColor.Color;
                style.Pattern = BackgroundType.Solid;

                worksheet.Cells["A1"].PutValue("Theme Color Example");
                worksheet.Cells["A1"].SetStyle(style);

                // Save the workbook
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

### See Also

* class [ThemeColor](../../themecolor/)
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


