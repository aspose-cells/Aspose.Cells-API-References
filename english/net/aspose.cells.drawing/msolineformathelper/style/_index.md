---
title: MsoLineFormatHelper.Style
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormatHelper property. Returns a Style object that represents the style of the specified range
type: docs
url: /net/aspose.cells.drawing/msolineformathelper/style/
---
## MsoLineFormatHelper.Style property

Returns a Style object that represents the style of the specified range.

```csharp
public MsoLineStyle Style { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineFormatHelperPropertyStyleDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a line shape to the worksheet
            var line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Get the MsoLineFormat for the line
            MsoLineFormat lineFormat = line.LineFormat;

            // Display the current line style
            Console.WriteLine("Current line style: " + lineFormat.Style);

            // Set properties to make the line visible and styled
            lineFormat.IsVisible = true;
            lineFormat.ForeColor = System.Drawing.Color.Red;
            lineFormat.Weight = 3; // 3 pt weight
            lineFormat.DashStyle = MsoLineDashStyle.Solid;

            // Change the line style to ThickBetweenThin
            lineFormat.Style = MsoLineStyle.ThickBetweenThin;
            Console.WriteLine("Line style changed to: " + lineFormat.Style);

            // Add another line with different style for comparison
            var line2 = worksheet.Shapes.AddLine(5, 15, 100, 15, 10, 100);
            line2.LineFormat.IsVisible = true;
            line2.LineFormat.ForeColor = System.Drawing.Color.Blue;
            line2.LineFormat.Weight = 3;
            line2.LineFormat.Style = MsoLineStyle.ThinThick;

            // Save the workbook to demonstrate the line style changes
            workbook.Save("MsoLineFormatHelperStyleDemo.xlsx");
        }
    }
}
```

### See Also

* enum [MsoLineStyle](../../msolinestyle/)
* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


