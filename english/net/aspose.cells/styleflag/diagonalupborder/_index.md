---
title: StyleFlag.DiagonalUpBorder
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Diagonal up border settings will be applied
type: docs
url: /net/aspose.cells/styleflag/diagonalupborder/
---
## StyleFlag.DiagonalUpBorder property

Diagonal up border settings will be applied.

```csharp
public bool DiagonalUpBorder { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.StyleFlagPropertyDiagonalUpBorderDemo
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleFlagPropertyDiagonalUpBorderDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access cell A1 and set some text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Create a style object and set diagonal up border
            Style style = workbook.CreateStyle();
            style.Borders.DiagonalStyle = CellBorderType.MediumDashDot;
            style.Borders.DiagonalColor = Color.Red;

            // Create a style flag and enable diagonal up border flag
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.DiagonalUpBorder = true;

            // Apply the style with the flag to the cell
            cell.SetStyle(style, styleFlag);

            // Create another cell to demonstrate the effect
            Cell cell2 = worksheet.Cells["B2"];
            cell2.PutValue("Diagonal Up Border Demo");

            // Create a different style for comparison
            Style style2 = workbook.CreateStyle();
            style2.Borders.DiagonalStyle = CellBorderType.Thick;
            style2.Borders.DiagonalColor = Color.Blue;

            // Apply the second style with the same flag
            cell2.SetStyle(style2, styleFlag);

            // Save the workbook
            workbook.Save("StyleFlagPropertyDiagonalUpBorderDemo.xlsx");
        }
    }
}
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


