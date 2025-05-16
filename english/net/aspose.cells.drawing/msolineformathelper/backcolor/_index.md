---
title: MsoLineFormatHelper.BackColor
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormatHelper property. Gets and sets the border line back color
type: docs
url: /net/aspose.cells.drawing/msolineformathelper/backcolor/
---
## MsoLineFormatHelper.BackColor property

Gets and sets the border line back color.

```csharp
public Color BackColor { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.MsoLineFormatHelperPropertyBackColorDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyBackColorDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a line shape to the worksheet
            var line = worksheet.Shapes.AddLine(5, 5, 100, 100, 5, 5);
            
            // Get the MsoLineFormat instance
            MsoLineFormat lineFormat = line.LineFormat;

            // Display the current BackColor value
            Console.WriteLine("Current BackColor value: " + lineFormat.BackColor);

            // Set a new BackColor value
            lineFormat.BackColor = Color.LightBlue;

            // Set other line properties to make the effect visible
            lineFormat.Style = MsoLineStyle.Single;
            lineFormat.Weight = 3;
            lineFormat.IsVisible = true;

            // Display the new BackColor value
            Console.WriteLine("New BackColor value: " + lineFormat.BackColor);

            // Add another line with different BackColor for comparison
            var line2 = worksheet.Shapes.AddLine(15, 5, 100, 100, 5, 5);
            line2.LineFormat.BackColor = Color.Pink;
            line2.LineFormat.Style = MsoLineStyle.Single;
            line2.LineFormat.Weight = 3;
            line2.LineFormat.IsVisible = true;

            // Save the workbook
            workbook.Save("MsoLineFormatHelperPropertyBackColorDemo.xlsx");
        }
    }
}
```

### See Also

* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


