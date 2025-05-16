---
title: MsoFillFormatHelper.IsVisible
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormatHelper property. Indicates whether there is fill
type: docs
url: /net/aspose.cells.drawing/msofillformathelper/isvisible/
---
## MsoFillFormatHelper.IsVisible property

Indicates whether there is fill.

```csharp
public bool IsVisible { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.MsoFillFormatHelperPropertyIsVisibleDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a rectangle shape
            var rectangle = worksheet.Shapes.AddRectangle(0, 0, 10, 10, 100, 100);
            MsoFillFormat fill = rectangle.FillFormat;

            // Configure visible fill with blue color
            fill.ForeColor = Color.Blue;
            fill.Transparency = 0;

            // Display initial visibility state
            Console.WriteLine("Initial IsVisible value: " + fill.IsVisible);

            // Save visible state for verification
            workbook.Save("VisibleFillDemo.xlsx");

            // Toggle fill visibility
            fill.IsVisible = false;
            Console.WriteLine("Updated IsVisible value: " + fill.IsVisible);

            // Save with hidden fill to demonstrate effect
            workbook.Save("HiddenFillDemo.xlsx");
        }
    }
}
```

### See Also

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


