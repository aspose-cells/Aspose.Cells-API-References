---
title: MsoLineFormatHelper.DashStyle
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormatHelper property. Gets or sets the dash style for the specified line
type: docs
url: /net/aspose.cells.drawing/msolineformathelper/dashstyle/
---
## MsoLineFormatHelper.DashStyle property

Gets or sets the dash style for the specified line.

```csharp
public MsoLineDashStyle DashStyle { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineFormatHelperPropertyDashStyleDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a line shape to demonstrate DashStyle
            var line = worksheet.Shapes.AddLine(5, 5, 100, 5, 200, 0);
            
            // Get the MsoLineFormat for the line
            MsoLineFormat lineFormat = line.LineFormat;

            // Display the current DashStyle value
            Console.WriteLine("Current DashStyle value: " + lineFormat.DashStyle);

            // Set different dash styles and observe the effects
            lineFormat.DashStyle = MsoLineDashStyle.Dash;
            Console.WriteLine("Line set to Dash style");

            lineFormat.DashStyle = MsoLineDashStyle.DashDot;
            Console.WriteLine("Line set to DashDot style");

            lineFormat.DashStyle = MsoLineDashStyle.DashDotDot;
            Console.WriteLine("Line set to DashDotDot style");

            lineFormat.DashStyle = MsoLineDashStyle.Solid;
            Console.WriteLine("Line set to Solid style");

            // Set line properties for better visibility
            lineFormat.ForeColor = System.Drawing.Color.Blue;
            lineFormat.Weight = 3; // 3 pt weight

            // Save the workbook to see the effects
            workbook.Save("PropertyDashStyleDemo.xlsx");
        }
    }
}
```

### See Also

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


