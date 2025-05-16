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
namespace AsposeCellsExamples.DrawingClassMsoLineFormatHelperDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassMsoLineFormatHelperDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a line shape to demonstrate MsoLineFormatHelper
            var line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Get the MsoLineFormat instance from the line
            MsoLineFormat lineFormat = line.LineFormat;

            // Configure line properties
            lineFormat.IsVisible = true;
            lineFormat.Style = MsoLineStyle.Single;
            lineFormat.ForeColor = Color.Red;
            lineFormat.BackColor = Color.White;
            lineFormat.DashStyle = MsoLineDashStyle.DashDotDot;
            lineFormat.Transparency = 0.5;
            lineFormat.Weight = 3.0;

            // Add another shape to demonstrate integration
            var rectangle = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            rectangle.LineFormat.ForeColor = Color.Blue;
            rectangle.LineFormat.Weight = 2.5;

            // Save the result
            workbook.Save("MsoLineFormatHelperDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


