---
title: PatternFill.BackgroundCellsColor
second_title: Aspose.Cells for .NET API Reference
description: PatternFill property. Gets and sets the foreground CellsColor object
type: docs
url: /net/aspose.cells.drawing/patternfill/backgroundcellscolor/
---
## PatternFill.BackgroundCellsColor property

Gets and sets the foreground [`CellsColor`](../../../aspose.cells/cellscolor/) object.

```csharp
public CellsColor BackgroundCellsColor { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PatternFillPropertyBackgroundCellsColorDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access cell A1 and set value for visibility
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Background Color Demo");

            // Get cell's style and configure pattern fill
            Style style = cell.GetStyle();
            style.Pattern = BackgroundType.Solid;

            // Display initial BackgroundColor state
            Console.WriteLine("Initial BackgroundColor: " + 
                              style.BackgroundColor.ToString());

            // Create and configure new background color
            CellsColor bgColor = workbook.CreateCellsColor();
            bgColor.ColorIndex = 44; // Light blue color index

            // Apply new background color and pattern
            style.BackgroundColor = bgColor.Color;

            // Apply modified style to cell
            cell.SetStyle(style);

            // Save and demonstrate result
            workbook.Save("PatternFillBackgroundDemo.xlsx");
            Console.WriteLine("Background color applied. Check output file.");
        }
    }
}
```

### See Also

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


