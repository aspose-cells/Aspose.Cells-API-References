---
title: PatternFill.ForegroundCellsColor
second_title: Aspose.Cells for .NET API Reference
description: PatternFill property. Gets and sets the foreground CellsColor object
type: docs
url: /net/aspose.cells.drawing/patternfill/foregroundcellscolor/
---
## PatternFill.ForegroundCellsColor property

Gets and sets the foreground [`CellsColor`](../../../aspose.cells/cellscolor/) object.

```csharp
public CellsColor ForegroundCellsColor { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyForegroundCellsColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Foreground Color Demo");

            Style style = workbook.CreateStyle();
            
            // Set background pattern type directly on the Style
            style.Pattern = BackgroundType.Solid;
            
            // Set foreground color directly using Style's built-in properties
            style.ForegroundColor = Color.Green;

            // Apply the style to the cell
            cell.SetStyle(style);

            workbook.Save("PatternFillForegroundDemo.xlsx");
        }
    }
}
```

### See Also

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


