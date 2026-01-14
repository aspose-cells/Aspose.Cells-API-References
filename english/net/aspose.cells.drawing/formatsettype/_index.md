---
title: Enum FormatSetType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.FormatSetType enum. Fill format set type
type: docs
url: /net/aspose.cells.drawing/formatsettype/
---
## FormatSetType enumeration

Fill format set type.

```csharp
public enum FormatSetType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No Fill format. |
| IsGradientSet | `1` | Gradient fill format. |
| IsTextureSet | `2` | Texture fill format. |
| IsPatternSet | `3` | Pattern fill format. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassFormatSetTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add a shape to demonstrate fill format
                Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 200);
                FillFormat fillFormat = shape.Fill;

                // Display initial fill type
                Console.WriteLine("Initial fill type: " + fillFormat.Type);

                // Demonstrate FormatSetType enum values
                Console.WriteLine("FormatSetType.None: " + (int)FormatSetType.None);
                Console.WriteLine("FormatSetType.IsGradientSet: " + (int)FormatSetType.IsGradientSet);
                Console.WriteLine("FormatSetType.IsTextureSet: " + (int)FormatSetType.IsTextureSet);
                Console.WriteLine("FormatSetType.IsPatternSet: " + (int)FormatSetType.IsPatternSet);

                // Apply different fill types using FormatSetType
                fillFormat.Type = (FillType)FormatSetType.IsGradientSet;
                Console.WriteLine("After setting gradient: " + fillFormat.Type);

                fillFormat.Type = (FillType)FormatSetType.IsPatternSet;
                Console.WriteLine("After setting pattern: " + fillFormat.Type);

                // Save the workbook
                workbook.Save("FormatSetTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with FormatSetType: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


