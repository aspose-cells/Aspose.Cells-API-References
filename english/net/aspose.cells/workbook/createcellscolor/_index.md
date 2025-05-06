---
title: Workbook.CreateCellsColor
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Creates a CellsColor object
type: docs
url: /net/aspose.cells/workbook/createcellscolor/
---
## Workbook.CreateCellsColor method

Creates a [`CellsColor`](../../cellscolor/) object.

```csharp
public CellsColor CreateCellsColor()
```

### Return Value

Returns a [`CellsColor`](../../cellscolor/) object.

### Examples

```csharp
// Called: CellsColor cellsColor = workbook.CreateCellsColor();
public static void Method_CreateCellsColor()
        {
            // Instantiate a new Workbook
            Workbook workbook = new Workbook();
            // Add a new worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Accessing a cell from the worksheet
            Cell cell = worksheet.Cells[&quot;B2&quot;];
            Style style = cell.GetStyle();

            // Setting the foreground color to yellow
            style.BackgroundColor = Color.Yellow;
            // Setting the background pattern to solid
            style.Pattern = BackgroundType.Solid;
            // Saving the modified style to the &quot;B2&quot; cell
            cell.SetStyle(style);

            // Adding custom color to the palette at 55th index
            Color customColor = Color.FromArgb(212, 213, 0);
            workbook.ChangePalette(customColor, 55);

            // Accessing another cell from the worksheet
            cell = worksheet.Cells[&quot;B3&quot;];
            // Adding some value to the cell
            cell.PutValue(&quot;Hello Aspose!&quot;);

            // Creating a CellsColor object
            CellsColor cellsColor = workbook.CreateCellsColor();

            // Setting the RGB color
            cellsColor.Color = Color.Red;

            // Applying the color to a cell
            cell = worksheet.Cells[&quot;B4&quot;];
            style = cell.GetStyle();
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;
            cell.SetStyle(style);

            // Save the workbook
            workbook.Save(&quot;ColorTypeExample.xlsx&quot;);
            workbook.Save(&quot;ColorTypeExample.pdf&quot;);
            return;
        }
```

### See Also

* class [CellsColor](../../cellscolor/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


