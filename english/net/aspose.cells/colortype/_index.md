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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassColorTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook for demonstration
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Demonstrate using ColorType enum values
                ColorType automatic = ColorType.Automatic;
                ColorType rgb = ColorType.RGB;
                ColorType theme = ColorType.Theme;

                // Display the enum values
                Console.WriteLine($"Automatic color type value: {(int)automatic}");
                Console.WriteLine($"RGB color type value: {(int)rgb}");
                Console.WriteLine($"Theme color type value: {(int)theme}");

                // Create a cell and set its value
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("ColorType Demo");

                // Create a style and apply it to the cell
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Black;
                cell.SetStyle(style);

                // Save the workbook
                workbook.Save("ColorTypeDemo.xlsx");

                Console.WriteLine("ColorType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ColorType demonstration: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


