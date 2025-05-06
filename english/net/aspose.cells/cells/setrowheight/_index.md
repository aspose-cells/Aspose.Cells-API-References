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
// Called: cells.SetRowHeight(2, -0.1);
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void Method_Double_()
        {
            caseName = &quot;testRowHeight_Exception_001&quot;;
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.SetRowHeight(2, -0.1);
            string msg = message + &quot;cells.SetRowHeight(2, -0.1)&quot;;
            writeToExcel(caseName, msg);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


