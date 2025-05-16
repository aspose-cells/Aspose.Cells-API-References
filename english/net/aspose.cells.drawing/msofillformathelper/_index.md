---
title: Class MsoFillFormatHelper
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.MsoFillFormatHelper class. Represents fill formatting for a shape
type: docs
url: /net/aspose.cells.drawing/msofillformathelper/
---
## MsoFillFormatHelper class

Represents fill formatting for a shape.

```csharp
public class MsoFillFormatHelper
```

## Properties

| Name | Description |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msofillformathelper/backcolor/) { get; set; } | Gets and sets the file back color. |
| [ForeColor](../../aspose.cells.drawing/msofillformathelper/forecolor/) { get; set; } | Gets and sets the fill fore color. |
| [ForeColorTransparency](../../aspose.cells.drawing/msofillformathelper/forecolortransparency/) { get; set; } | Returns or sets the degree of fore color of the specified fill as a value from 0.0 (opaque) through 1.0 (clear). |
| [ImageData](../../aspose.cells.drawing/msofillformathelper/imagedata/) { get; set; } | Gets and sets the Texture and Picture fill data. |
| [IsVisible](../../aspose.cells.drawing/msofillformathelper/isvisible/) { get; set; } | Indicates whether there is fill. |
| [Texture](../../aspose.cells.drawing/msofillformathelper/texture/) { get; } | Gets the texture fill type. |

## Methods

| Name | Description |
| --- | --- |
| [SetOneColorGradient](../../aspose.cells.drawing/msofillformathelper/setonecolorgradient/)(Color, double, GradientStyleType, int) | Sets the specified fill to a one-color gradient. |

### Examples

```csharp
namespace AsposeCellsExamples.DrawingClassMsoFillFormatHelperDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassMsoFillFormatHelperDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape to demonstrate fill formatting
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 10, 10, 200, 150);

            // Get MsoFillFormat instance from the shape
            MsoFillFormat fillFormat = shape.FillFormat;

            // Configure solid fill properties
            fillFormat.ForeColor = Color.LightBlue;
            fillFormat.BackColor = Color.DarkBlue;
            fillFormat.Transparency = 0.3; // Fixed property name
            fillFormat.IsVisible = true;

            // Apply gradient fill
            fillFormat.SetOneColorGradient(Color.Green, 0.8, GradientStyleType.DiagonalUp, 2);

            // Save the modified workbook
            workbook.Save("MsoFillFormatHelperDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


