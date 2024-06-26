---
title: WebWorksheet.FreezePanes
second_title: Aspose.Cells for .NET API Reference
description: WebWorksheet method. Freezes panes at the specified cell in the worksheet
type: docs
url: /net/aspose.cells.gridweb.data/webworksheet/freezepanes/
---
## WebWorksheet.FreezePanes method

Freezes panes at the specified cell in the worksheet.

```csharp
public void FreezePanes(int row, int column, int freezedRows, int freezedColumns)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |
| column | Int32 | Column index. |
| freezedRows | Int32 | Number of visible rows in top pane, no more than row index. |
| freezedColumns | Int32 | Number of visible columns in left pane, no more than column index. |

### Remarks

Row index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.

The first two parameters specify the freezed position and the last two parameters specify the area freezed on the left top pane.

### See Also

* class [WebWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


