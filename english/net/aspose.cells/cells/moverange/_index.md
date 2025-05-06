---
title: Cells.MoveRange
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Moves the range
type: docs
url: /net/aspose.cells/cells/moverange/
---
## Cells.MoveRange method

Moves the range.

```csharp
public void MoveRange(CellArea sourceArea, int destRow, int destColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceArea | CellArea | The range which should be moved. |
| destRow | Int32 | The dest row. |
| destColumn | Int32 | The dest column. |

### Examples

```csharp
// Called: cells.MoveRange(cellarea, 0, -1);
[Test, Ignore(&quot;Not ready to test this yet&quot;)]
        public void Method_Int32_()
        {
            caseName = &quot;testMoveRange_Exception_002&quot;;
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            CellArea cellarea = common.setCellArea(0, 0, 1, 1);
            cells.MoveRange(cellarea, 0, -1);
            string msg = message + &quot;cells.MoveRange(cellarea, 0, -1)&quot;;
            writeToExcel(caseName, msg);
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


