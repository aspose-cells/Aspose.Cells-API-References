---
title: Cells.SetRowHeight
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Sets the height of the specified row
type: docs
url: /net/aspose.cells/cells/setrowheight/
---
## Cells.SetRowHeight method

Sets the height of the specified row.

```csharp
public void SetRowHeight(int row, double height)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |
| height | Double | Height of row.In unit of point It should be between 0 and 409.5. |

### Examples

```csharp
// Called: cells.SetRowHeight(0, 410);
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void Cells_Method_SetRowHeight()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.SetRowHeight(0, 410);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


