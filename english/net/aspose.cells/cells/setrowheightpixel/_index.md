---
title: Cells.SetRowHeightPixel
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Sets row height in unit of pixels
type: docs
url: /net/aspose.cells/cells/setrowheightpixel/
---
## Cells.SetRowHeightPixel method

Sets row height in unit of pixels.

```csharp
public void SetRowHeightPixel(int row, int pixels)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |
| pixels | Int32 | Number of pixels. |

### Examples

```csharp
// Called: worksheet.Cells.SetRowHeightPixel(0, int.MaxValue);
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void Cells_Method_SetRowHeightPixel()
        {
            Workbook workbook = new Workbook();
            //Access first sheet 
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells.SetColumnWidthPixel(0, int.MaxValue);

            worksheet.Cells.SetRowHeightPixel(0, int.MaxValue);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


