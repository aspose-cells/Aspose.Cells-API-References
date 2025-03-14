---
title: Cells.GetCellDisplayStyle
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Get the display style of given cell
type: docs
url: /net/aspose.cells/cells/getcelldisplaystyle/
---
## GetCellDisplayStyle(int, int) {#getcelldisplaystyle}

Get the display style of given cell.

```csharp
public Style GetCellDisplayStyle(int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | row index of given cell |
| column | Int32 | column of given cell |

### Return Value

the display style of given cell.

### Remarks

Same with [`GetDisplayStyle`](../../cell/getdisplaystyle/), and same with using SideBorders for `GetCellDisplayStyle`.

### See Also

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCellDisplayStyle(int, int, BorderType) {#getcelldisplaystyle_1}

Get the display style of given cell.

```csharp
public Style GetCellDisplayStyle(int row, int column, BorderType adjacentBorders)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | row index of given cell |
| column | Int32 | column of given cell |
| adjacentBorders | BorderType | Indicates which borders need to be checked and adjusted according to the borders of adjacent cells. Please see the description for the same parameter of [`GetDisplayStyle`](../../cell/getdisplaystyle/). |

### Return Value

the display style of given cell.

### Remarks

If the cell is also affected by other settings such as conditional formatting, list objects, etc., then the display style may be different from [`GetCellStyle`](../getcellstyle/). And because those settings also may be applied to empty(non-existing) cells, using this method can avoid the instantiation of those empty cells so the performance will be better than getting the Cell instance from Cells and then calling [`GetDisplayStyle`](../../cell/getdisplaystyle/).

### See Also

* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


