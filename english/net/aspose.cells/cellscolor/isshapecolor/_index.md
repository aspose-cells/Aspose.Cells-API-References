---
title: CellsColor.IsShapeColor
second_title: Aspose.Cells for .NET API Reference
description: CellsColor property. Gets and set the color which should apply to cell or shape
type: docs
url: /net/aspose.cells/cellscolor/isshapecolor/
---
## CellsColor.IsShapeColor property

Gets and set the color which should apply to cell or shape.

```csharp
public bool IsShapeColor { get; set; }
```

### Remarks

The expression of the color of the cell and the shape is different. For example: the theme color with same tint value will be not same in the cell and the shape.

### Examples

```csharp
// Called: cellsColor.IsShapeColor = false;
public static void CellsColor_Property_IsShapeColor()
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


