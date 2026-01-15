---
title: Enum GradientColorType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.GradientColorType enum. Represents the gradient color type for the specified fill
type: docs
url: /net/aspose.cells.drawing/gradientcolortype/
---
## GradientColorType enumeration

Represents the gradient color type for the specified fill.

```csharp
public enum GradientColorType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No gradient color |
| OneColor | `1` | One gradient color |
| PresetColors | `2` | Preset gradient colors |
| TwoColors | `3` | Two gradient colors |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassGradientColorTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add a shape to demonstrate gradient fill
                Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);
                FillFormat fill = shape.Fill;

                // Set gradient fill type
                fill.FillType = FillType.Gradient;

                // Demonstrate different GradientColorType enum values
                Console.WriteLine("Available GradientColorType values:");
                Console.WriteLine("None: " + GradientColorType.None);
                Console.WriteLine("OneColor: " + GradientColorType.OneColor);
                Console.WriteLine("PresetColors: " + GradientColorType.PresetColors);
                Console.WriteLine("TwoColors: " + GradientColorType.TwoColors);

                // Read and display the current gradient color type (property is read-only)
                Console.WriteLine("Current gradient color type: " + fill.GradientColorType);

                // Save the workbook
                workbook.Save("GradientColorTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GradientColorType: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


