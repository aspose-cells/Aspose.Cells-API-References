---
title: Cells.GetColumnWidthPixel
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the width of the specified column in normal view in units of pixel
type: docs
url: /net/aspose.cells/cells/getcolumnwidthpixel/
---
## GetColumnWidthPixel(int) {#getcolumnwidthpixel}

Gets the width of the specified column in normal view, in units of pixel.

```csharp
public int GetColumnWidthPixel(int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index |

### Return Value

Width of column in normal view.

### Examples

```csharp
// Called: int t = ws2.Cells.GetColumnWidthPixel(1);
public void Cells_Method_GetColumnWidthPixel()
{
    var workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    var ws = workbook.Worksheets[0];
    var ws2 = workbook.Worksheets[1];
    var fromRange = ws.Cells.CreateRange(0, 0, 10, 10);
    int t = ws2.Cells.GetColumnWidthPixel(1);
    var toRange = ws2.Cells.CreateRange(0, 0, 10, 10);
    toRange.Copy(fromRange, new PasteOptions() { PasteType = PasteType.Default });
    Assert.AreEqual(t, ws2.Cells.GetColumnWidthPixel(1));
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetColumnWidthPixel(int, bool) {#getcolumnwidthpixel_1}

Gets the width of the specified column in normal view, in units of pixel.

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int GetColumnWidthPixel(int column, bool original)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index |
| original | Boolean | Indicates whether returning original width even when the column is hidden |

### Return Value

Width of column in normal view.

### Remarks

NOTE: This method is now obsolete. Instead, please use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples.CellsMethodGetColumnWidthPixelWithInt32BooleanDemo
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnWidthPixelWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Create a new workbook and access first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Set standard column width to 80 pixels
            worksheet.Cells.StandardWidthPixels = 80;

            // Set specific column width for column 2 (third column) to 120 pixels
            worksheet.Cells.SetColumnWidthPixel(2, 120);

            try
            {
                // Get current width with user modifications (original: false)
                int currentWidth = worksheet.Cells.GetColumnWidthPixel(2, false);
                Console.WriteLine($"Column 2 current width: {currentWidth} pixels");

                // Get original width without modifications (original: true)
                int originalWidth = worksheet.Cells.GetColumnWidthPixel(2, true);
                Console.WriteLine($"Column 2 original width: {originalWidth} pixels");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnWidthPixel: {ex.Message}");
            }

            // Save the workbook to demonstrate column width persistence
            workbook.Save("ColumnWidthDemo.xlsx");
        }
    }
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


