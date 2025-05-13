---
title: CellsColor.Transparency
second_title: Aspose.Cells for .NET API Reference
description: CellsColor property. Gets and sets transparency as a value from 0.0 opaque through 1.0 clear
type: docs
url: /net/aspose.cells/cellscolor/transparency/
---
## CellsColor.Transparency property

Gets and sets transparency as a value from 0.0 (opaque) through 1.0 (clear).

```csharp
public double Transparency { get; set; }
```

### Examples

```csharp
// Called: cellsColor.Transparency = 0.5;
public static void CellsColor_Property_Transparency()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a range of cells
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A10");

            // Create a CellsColor instance
            CellsColor cellsColor = workbook.CreateCellsColor();

            // Set properties of CellsColor
            cellsColor.IsShapeColor = false;
            cellsColor.Color = Color.Red;
            cellsColor.ColorIndex = 5;
            cellsColor.Argb = Color.Blue.ToArgb();
            cellsColor.Transparency = 0.5;

            // Apply the CellsColor to the range
            Style style = workbook.CreateStyle();
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;
            range.ApplyStyle(style, new StyleFlag { CellShading = true });

            // Save the workbook
            workbook.Save("CellsColorExample.xlsx");
            workbook.Save("CellsColorExample.pdf");
        }
```

### See Also

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


