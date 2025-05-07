---
title: Range.ApplyStyle
second_title: Aspose.Cells for .NET API Reference
description: Range method. Applies formats for a whole range
type: docs
url: /net/aspose.cells/range/applystyle/
---
## Range.ApplyStyle method

Applies formats for a whole range.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### Remarks

Each cell in this range will contains a [`Style`](../../style/) object. So this is a memory-consuming method. Please use it carefully.

### Examples

```csharp
// Called: range.ApplyStyle(style, new StyleFlag { CellShading = true });
public static void Method_StyleFlag_()
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

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


