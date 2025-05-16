---
title: Style.SetBorder
second_title: Aspose.Cells for .NET API Reference
description: Style method. Sets the borders of the style
type: docs
url: /net/aspose.cells/style/setborder/
---
## SetBorder(BorderType, CellBorderType, Color) {#setborder_1}

Sets the borders of the style.

```csharp
public bool SetBorder(BorderType borderType, CellBorderType borderStyle, Color borderColor)
```

| Parameter | Type | Description |
| --- | --- | --- |
| borderType | BorderType | The border(s) to be set, can be combination of [`BorderType`](../../bordertype/). |
| borderStyle | CellBorderType | The style of the border. |
| borderColor | Color | The color of the border. |

### Return Value

Whether current border settings have been changed.

### Examples

```csharp
// Called: style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Black);
public static void Style_Method_SetBorder()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            // Create a range of cells
            var range = worksheet.Cells.CreateRange("A1:D4");

            // Create a style object
            Style style = workbook.CreateStyle();
            // Set the borders for the range
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.DiagonalDown, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.DiagonalUp, CellBorderType.Thin, Color.Blue);

            // Apply the style to the range
            StyleFlag flag = new StyleFlag { Borders = true };
            range.ApplyStyle(style, flag);

            // Save the workbook
            workbook.Save("BorderTypeExample.xlsx");
            workbook.Save("BorderTypeExample.pdf");
        }
```

### See Also

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetBorder(BorderType, CellBorderType, CellsColor) {#setborder}

Sets the borders of the style.

```csharp
public bool SetBorder(BorderType borderType, CellBorderType borderStyle, CellsColor borderColor)
```

| Parameter | Type | Description |
| --- | --- | --- |
| borderType | BorderType | The border(s) to be set, can be combination of [`BorderType`](../../bordertype/). |
| borderStyle | CellBorderType | The style of the border. |
| borderColor | CellsColor | The color of the border. |

### Return Value

Whether current border settings have been changed.

### Examples

```csharp
namespace AsposeCellsExamples.StyleMethodSetBorderWithBorderTypeCellBorderTypeCellsCDemo
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleMethodSetBorderWithBorderTypeCellBorderTypeCellsCDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add some data for context
            worksheet.Cells["A1"].Value = "Border Demo";
            
            try
            {
                // Create a style
                Style style = workbook.CreateStyle();
                
                // Create a CellsColor object using the proper factory method
                CellsColor borderColor = workbook.CreateCellsColor();
                borderColor.Color = Color.Green;
                
                // Call SetBorder with BorderType, CellBorderType and CellsColor parameters
                bool result = style.SetBorder(
                    BorderType.TopBorder, 
                    CellBorderType.Thick, 
                    borderColor);
                
                // Apply the style to a cell
                worksheet.Cells["A1"].SetStyle(style);
                
                Console.WriteLine("SetBorder method called successfully. Result: " + result);
                
                // Save the workbook
                workbook.Save("SetBorderDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetBorder: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


