---
title: MsoLineFormatHelper.IsVisible
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormatHelper property. Indicates whether the object is visible
type: docs
url: /net/aspose.cells.drawing/msolineformathelper/isvisible/
---
## MsoLineFormatHelper.IsVisible property

Indicates whether the object is visible.

```csharp
public bool IsVisible { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.MsoLineFormatHelperPropertyIsVisibleDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a line shape to the worksheet
            var line = worksheet.Shapes.AddLine(5, 5, 100, 100, 200, 0);
            
            // Get the MsoLineFormat instance
            MsoLineFormat lineFormat = line.LineFormat;

            // Display current visibility status
            Console.WriteLine("Line is currently visible: " + lineFormat.IsVisible);

            // Make the line invisible
            lineFormat.IsVisible = false;
            Console.WriteLine("Line visibility after setting to false: " + lineFormat.IsVisible);

            // Change line properties to make it more visible when we show it again
            lineFormat.Style = MsoLineStyle.Single;
            lineFormat.ForeColor = Color.Red;
            lineFormat.Weight = 3;

            // Make the line visible again
            lineFormat.IsVisible = true;
            Console.WriteLine("Line visibility after setting to true: " + lineFormat.IsVisible);

            // Save the workbook
            workbook.Save("MsoLineFormatHelperPropertyIsVisibleDemo.xlsx");
        }
    }
}
```

### See Also

* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


