---
title: MsoLineFormatHelper.ForeColor
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormatHelper property. Gets and sets the border line fore color
type: docs
url: /net/aspose.cells.drawing/msolineformathelper/forecolor/
---
## MsoLineFormatHelper.ForeColor property

Gets and sets the border line fore color.

```csharp
public Color ForeColor { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.MsoLineFormatHelperPropertyForeColorDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyForeColorDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add three line shapes to demonstrate different ForeColor settings
            var line1 = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);
            var line2 = worksheet.Shapes.AddLine(5, 20, 100, 20, 10, 100);
            var line3 = worksheet.Shapes.AddLine(5, 35, 100, 35, 10, 100);

            // Get MsoLineFormat for each line
            MsoLineFormat lineFormat1 = line1.LineFormat;
            MsoLineFormat lineFormat2 = line2.LineFormat;
            MsoLineFormat lineFormat3 = line3.LineFormat;

            // Display default ForeColor value
            Console.WriteLine("Default ForeColor value: " + lineFormat1.ForeColor);

            // Set different ForeColor values for each line
            lineFormat1.ForeColor = Color.Red;
            lineFormat1.Weight = 3;
            lineFormat1.Style = MsoLineStyle.Single;

            lineFormat2.ForeColor = Color.Green;
            lineFormat2.Weight = 3;
            lineFormat2.Style = MsoLineStyle.Single;

            lineFormat3.ForeColor = Color.Blue;
            lineFormat3.Weight = 3;
            lineFormat3.Style = MsoLineStyle.Single;

            // Add a text box to explain the colors
            var textbox = worksheet.Shapes.AddTextBox(5, 50, 200, 50, 200, 100);
            textbox.Text = "Line Colors:\n1. Red\n2. Green\n3. Blue";

            // Save the workbook to show the ForeColor effects
            workbook.Save("MsoLineFormatHelperPropertyForeColorDemo.xlsx");
        }
    }
}
```

### See Also

* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


