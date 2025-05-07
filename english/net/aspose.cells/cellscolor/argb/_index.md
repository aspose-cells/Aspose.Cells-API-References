---
title: CellsColor.Argb
second_title: Aspose.Cells for .NET API Reference
description: CellsColor property. Gets and sets the color from a 32bit ARGB value
type: docs
url: /net/aspose.cells/cellscolor/argb/
---
## CellsColor.Argb property

Gets and sets the color from a 32-bit ARGB value.

```csharp
public int Argb { get; set; }
```

### Examples

```csharp
// Called: cellsColor.Argb = Color.Blue.ToArgb();
public static void Property_Argb()
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


