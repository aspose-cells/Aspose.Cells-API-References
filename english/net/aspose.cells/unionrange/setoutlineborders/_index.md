---
title: UnionRange.SetOutlineBorders
second_title: Aspose.Cells for .NET API Reference
description: UnionRange method. Sets out line borders around a range of cells
type: docs
url: /net/aspose.cells/unionrange/setoutlineborders/
---
## SetOutlineBorders(CellBorderType[], Color[]) {#setoutlineborders_1}

Sets out line borders around a range of cells.

```csharp
public void SetOutlineBorders(CellBorderType[] borderStyles, Color[] borderColors)
```

| Parameter | Type | Description |
| --- | --- | --- |
| borderStyles | CellBorderType[] | Border styles. |
| borderColors | Color[] | Border colors. |

### Remarks

Both the length of borderStyles and borderStyles must be 4. The order of borderStyles and borderStyles must be top,bottom,left,right

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class UnionRangeMethodSetOutlineBordersWithCellBorderTypeColorDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate some data in cells
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800);

            // Create a range instead of union range
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // Prepare border styles and colors
            CellBorderType[] borderStyles = new CellBorderType[]
            {
                CellBorderType.Thick,
                CellBorderType.Dotted,
                CellBorderType.Double,
                CellBorderType.Medium
            };

            Color[] borderColors = new Color[]
            {
                Color.Red,
                Color.Blue,
                Color.Green,
                Color.Purple
            };

            try
            {
                // Call SetOutlineBorders with CellBorderType[] and Color[] parameters
                range.SetOutlineBorders(borderStyles, borderColors);

                Console.WriteLine("SetOutlineBorders method executed successfully with parameters (CellBorderType[], Color[])");
                Console.WriteLine($"Borders applied to range: {range.RefersTo}");

                // Display range information
                Console.WriteLine($"\nRange Info - FirstRow: {range.FirstRow}, FirstColumn: {range.FirstColumn}");
                Console.WriteLine($"RowCount: {range.RowCount}, ColumnCount: {range.ColumnCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetOutlineBorders method: {ex.Message}");
            }

            // Save the workbook
            workbook.Save("UnionRangeSetOutlineBordersDemo.xlsx");
        }
    }
}
```

### See Also

* enum [CellBorderType](../../cellbordertype/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType, Color) {#setoutlineborders}

Sets the outline borders around a range of cells with same border style and color.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, Color borderColor)
```

| Parameter | Type | Description |
| --- | --- | --- |
| borderStyle | CellBorderType | Border style. |
| borderColor | Color | Border color. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class UnionRangeMethodSetOutlineBordersWithCellBorderTypeColorDemo1
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate some data in cells
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800);

            // Create a range
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            try
            {
                // Call SetOutlineBorders with CellBorderType and Color parameters
                range.SetOutlineBorders(CellBorderType.Thick, Color.Red);

                Console.WriteLine("SetOutlineBorders method executed successfully with parameters (CellBorderType.Thick, Color.Red)");
                Console.WriteLine($"Outline borders applied to range: {range.RefersTo}");

                // Display range information
                Console.WriteLine($"\nRange Info - FirstRow: {range.FirstRow}, FirstColumn: {range.FirstColumn}");
                Console.WriteLine($"RowCount: {range.RowCount}, ColumnCount: {range.ColumnCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetOutlineBorders method: {ex.Message}");
            }

            // Save the workbook
            workbook.Save("UnionRangeSetOutlineBordersDemo.xlsx");
        }
    }
}
```

### See Also

* enum [CellBorderType](../../cellbordertype/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


