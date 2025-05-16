---
title: MsoFillFormatHelper.ForeColor
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormatHelper property. Gets and sets the fill fore color
type: docs
url: /net/aspose.cells.drawing/msofillformathelper/forecolor/
---
## MsoFillFormatHelper.ForeColor property

Gets and sets the fill fore color.

```csharp
public Color ForeColor { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.MsoFillFormatHelperPropertyForeColorDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyForeColorDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a rectangle shape to access MsoFillFormatHelper
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);
            MsoFillFormat fillFormat = shape.FillFormat;

            // Enable fill visibility and set initial color
            fillFormat.IsVisible = true;
            fillFormat.ForeColor = Color.LightBlue;
            Console.WriteLine("Initial ForeColor: " + fillFormat.ForeColor);

            // Modify ForeColor and transparency
            fillFormat.ForeColor = Color.FromArgb(255, 0, 128, 0); // Dark green
            fillFormat.Transparency = 0.3; // Fixed property name
            Console.WriteLine("Modified ForeColor: " + fillFormat.ForeColor);

            // Add another shape for comparison
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 0, 0, 0, 100, 200);
            shape2.FillFormat.IsVisible = true;

            // Save the workbook with visual changes
            workbook.Save("MsoFillForeColorDemo.xlsx");
        }
    }
}
```

### See Also

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


