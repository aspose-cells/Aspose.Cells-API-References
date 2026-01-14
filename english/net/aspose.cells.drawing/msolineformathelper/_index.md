---
title: Class MsoLineFormatHelper
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.MsoLineFormatHelper class. Represents line and arrowhead formatting
type: docs
url: /net/aspose.cells.drawing/msolineformathelper/
---
## MsoLineFormatHelper class

Represents line and arrowhead formatting.

```csharp
public class MsoLineFormatHelper
```

## Properties

| Name | Description |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msolineformathelper/backcolor/) { get; set; } | Gets and sets the border line back color. |
| [DashStyle](../../aspose.cells.drawing/msolineformathelper/dashstyle/) { get; set; } | Gets or sets the dash style for the specified line. |
| [ForeColor](../../aspose.cells.drawing/msolineformathelper/forecolor/) { get; set; } | Gets and sets the border line fore color. |
| [IsVisible](../../aspose.cells.drawing/msolineformathelper/isvisible/) { get; set; } | Indicates whether the object is visible. |
| [Style](../../aspose.cells.drawing/msolineformathelper/style/) { get; set; } | Returns a Style object that represents the style of the specified range. |
| [Transparency](../../aspose.cells.drawing/msolineformathelper/transparency/) { get; set; } | Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear). |
| [Weight](../../aspose.cells.drawing/msolineformathelper/weight/) { get; set; } | Returns or sets the weight of the line ,in units of pt. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DrawingClassMsoLineFormatHelperDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Create a shape to demonstrate line formatting
                Shape shape = worksheet.Shapes.AddLine(10, 10, 100, 100, 0, 0);

                // Get the line format directly from the shape
                MsoLineFormat lineFormat = shape.LineFormat;

                // Set properties directly on the line format
                lineFormat.IsVisible = true;
                lineFormat.Style = MsoLineStyle.Single;
                lineFormat.ForeColor = Color.Blue;
                lineFormat.BackColor = Color.LightGray;
                lineFormat.DashStyle = MsoLineDashStyle.Solid;
                lineFormat.Transparency = 0.2;
                lineFormat.Weight = 2.5;

                // Display the configured properties
                Console.WriteLine($"Line is visible: {lineFormat.IsVisible}");
                Console.WriteLine($"Line style: {lineFormat.Style}");
                Console.WriteLine($"Fore color: {lineFormat.ForeColor}");
                Console.WriteLine($"Back color: {lineFormat.BackColor}");
                Console.WriteLine($"Dash style: {lineFormat.DashStyle}");
                Console.WriteLine($"Transparency: {lineFormat.Transparency}");
                Console.WriteLine($"Weight: {lineFormat.Weight}");

                // Save the workbook
                workbook.Save("MsoLineFormatHelperDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with MsoLineFormatHelper: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


