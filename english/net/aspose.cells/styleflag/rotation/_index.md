---
title: StyleFlag.Rotation
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Rotation setting will be applied
type: docs
url: /net/aspose.cells/styleflag/rotation/
---
## StyleFlag.Rotation property

Rotation setting will be applied.

```csharp
public bool Rotation { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.StyleFlagPropertyRotationDemo
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyRotationDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access cell A1 and set some text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Rotated Text");

            // Get the style of the cell
            Style style = cell.GetStyle();

            // Display current rotation value
            Console.WriteLine("Current Rotation value: " + style.RotationAngle);

            // Set new rotation value (45 degrees)
            style.RotationAngle = 45;

            // Create a style flag and enable rotation flag
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Rotation = true;

            // Apply the style with rotation to the cell
            cell.SetStyle(style, styleFlag);

            // Auto-fit the column to see the rotated text properly
            worksheet.AutoFitColumn(0);

            // Save the result
            workbook.Save("PropertyRotationDemo.xlsx");
        }
    }
}
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


