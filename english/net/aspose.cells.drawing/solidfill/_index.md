---
title: Class SolidFill
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.SolidFill class. Encapsulates the object that represents solid fill format
type: docs
url: /net/aspose.cells.drawing/solidfill/
---
## SolidFill class

Encapsulates the object that represents solid fill format

```csharp
public class SolidFill : Fill
```

## Properties

| Name | Description |
| --- | --- |
| [CellsColor](../../aspose.cells.drawing/solidfill/cellscolor/) { get; set; } | Gets and sets the [`CellsColor`](./cellscolor/) object. |
| [Color](../../aspose.cells.drawing/solidfill/color/) { get; set; } | Gets or sets the Color. |
| [Transparency](../../aspose.cells.drawing/solidfill/transparency/) { get; set; } | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |

## Methods

| Name | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/solidfill/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/solidfill/gethashcode/)() | Gets the hash code. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using System.Drawing;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;

    public class DrawingClassSolidFillDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            try
            {
                // Add a simple rectangle shape to the sheet
                Shape rect = sheet.Shapes.AddRectangle(2, 0, 2, 0, 150, 100);

                // Configure the shape to use a solid fill
                rect.Fill.FillType = FillType.Solid;

                // Obtain the SolidFill object
                SolidFill solidFill = rect.Fill.SolidFill;

                // Set solid fill properties
                solidFill.Color = Color.CornflowerBlue;   // System.Drawing.Color
                solidFill.Transparency = 0.25;            // 0 = opaque, 1 = fully transparent

                // Access the CellsColor property (read/write)
                CellsColor cellsColor = solidFill.CellsColor;
                if (cellsColor != null)
                {
                    Console.WriteLine("CellsColor object is available.");
                }
                else
                {
                    Console.WriteLine("CellsColor is null (default).");
                }

                Console.WriteLine($"SolidFill created with Color={solidFill.Color.Name}, Transparency={solidFill.Transparency}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SolidFill: {ex.Message}");
            }

            // Save the workbook to verify the shape appearance
            workbook.Save("DrawingClassSolidFillDemo.xlsx");
        }
    }
}
```

### See Also

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


