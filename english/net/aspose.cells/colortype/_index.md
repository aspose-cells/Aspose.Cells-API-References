---
title: Enum ColorType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ColorType enum. Represents all color type
type: docs
url: /net/aspose.cells/colortype/
---
## ColorType enumeration

Represents all color type

```csharp
public enum ColorType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Automatic | `0` | Automatic color. |
| AutomaticIndex | `1` | It's automatic color,but the displayed color depends the setting of the OS System. |
| RGB | `2` | The RGB color. |
| IndexedColor | `3` | The color index in the color palette. |
| Theme | `4` | The theme color. |

### Examples

```csharp
[C#]

namespace Demos
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColorTypeDemo
    {
        public static void ColorTypeExample()
        {
            // Instantiate a new Workbook
            Workbook workbook = new Workbook();
            // Add a new worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Accessing a cell from the worksheet
            Cell cell = worksheet.Cells["B2"];
            Style style = cell.GetStyle();

            // Setting the foreground color to yellow
            style.BackgroundColor = Color.Yellow;
            // Setting the background pattern to solid
            style.Pattern = BackgroundType.Solid;
            // Saving the modified style to the "B2" cell
            cell.SetStyle(style);

            // Adding custom color to the palette at 55th index
            Color customColor = Color.FromArgb(212, 213, 0);
            workbook.ChangePalette(customColor, 55);

            // Accessing another cell from the worksheet
            cell = worksheet.Cells["B3"];
            // Adding some value to the cell
            cell.PutValue("Hello Aspose!");

            // Creating a CellsColor object
            CellsColor cellsColor = workbook.CreateCellsColor();

            // Setting the RGB color
            cellsColor.Color = Color.Red;

            // Applying the color to a cell
            cell = worksheet.Cells["B4"];
            style = cell.GetStyle();
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;
            cell.SetStyle(style);

            // Save the workbook
            workbook.Save("ColorTypeExample.xlsx");
            workbook.Save("ColorTypeExample.pdf");
            return;
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


