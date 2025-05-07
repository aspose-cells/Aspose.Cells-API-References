---
title: Cells.SetColumnWidth
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Sets the width of the specified column in normal view
type: docs
url: /net/aspose.cells/cells/setcolumnwidth/
---
## Cells.SetColumnWidth method

Sets the width of the specified column in normal view.

```csharp
public void SetColumnWidth(int column, double width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |
| width | Double | Width of column.Column width must be between 0 and 255. |

### Remarks

To hide a column, sets column width to zero.

### Examples

```csharp
// Called: cells.SetColumnWidth(0, -0.2);
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void Method_Double_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.SetColumnWidth(0, -0.2);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


