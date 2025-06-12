---
title: TwoColorGradient.TwoColorGradient
second_title: Aspose.Cells for .NET API Reference
description: TwoColorGradient constructor. 
type: docs
url: /net/aspose.cells/twocolorgradient/twocolorgradient/
---
## TwoColorGradient constructor

```csharp
public TwoColorGradient(Color color1, Color color2, GradientStyleType gradientStyleType, 
    int variant)
```

| Parameter | Type | Description |
| --- | --- | --- |
| color1 | Color |  |
| color2 | Color |  |
| gradientStyleType | GradientStyleType |  |
| variant | Int32 |  |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class TwoColorGradientMethodCtorWithColorColorGradientStyleTypeIntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Create a custom style
                Style style = workbook.CreateStyle();

                // Apply two-color gradient using the correct API method
                style.SetTwoColorGradient(
                    Color.FromArgb(255, 255, 0, 0),     // Red color
                    Color.FromArgb(255, 0, 0, 255),     // Blue color
                    GradientStyleType.DiagonalDown,     // Gradient style
                    1                                   // Variant
                );

                // Apply style to cell and set sample text
                Cell cell = worksheet.Cells["B2"];
                cell.PutValue("Two-Color Gradient Demo");
                cell.SetStyle(style);

                // Adjust cell dimensions for visibility
                worksheet.Cells.SetRowHeight(1, 40);
                worksheet.Cells.SetColumnWidth(1, 30);

                Console.WriteLine("TwoColorGradient constructor executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing constructor: {ex.Message}");
            }

            workbook.Save("TwoColorGradientCtorDemo.xlsx");
        }
    }
}
```

### See Also

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


