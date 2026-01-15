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

    public class TwoColorGradientMethodSharpctorWithColorColorGradientStyleTyInt32Demo
    {
        public static void Run()
        {
            try
            {
                // Create a TwoColorGradient instance using the constructor with all parameters
                TwoColorGradient gradient = new TwoColorGradient(
                    Color.LightBlue,
                    Color.DarkBlue,
                    GradientStyleType.Horizontal,
                    1);

                // Display the gradient properties to verify initialization
                Console.WriteLine($"Gradient created with:");
                Console.WriteLine($"Color1: {gradient.Color1}");
                Console.WriteLine($"Color2: {gradient.Color2}");
                Console.WriteLine($"GradientStyleType: {gradient.GradientStyleType}");
                Console.WriteLine($"Variant: {gradient.Variant}");

                // Create a workbook and apply the gradient to demonstrate functionality
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Apply the gradient to a cell
                Style style = workbook.CreateStyle();
                style.SetTwoColorGradient(
                    gradient.Color1,
                    gradient.Color2,
                    gradient.GradientStyleType,
                    gradient.Variant);

                worksheet.Cells["A1"].PutValue("TwoColorGradient Demo");
                worksheet.Cells["A1"].SetStyle(style);

                // Save the workbook
                workbook.Save("TwoColorGradientDemo.xlsx");
                Console.WriteLine("Gradient applied successfully to workbook.");
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

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


