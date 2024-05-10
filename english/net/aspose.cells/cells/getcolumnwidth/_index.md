---
title: Cells.GetColumnWidth
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the column width
type: docs
url: /net/aspose.cells/cells/getcolumnwidth/
---
## GetColumnWidth(int, bool, CellsUnitType) {#getcolumnwidth_1}

Gets the column width.

```csharp
public double GetColumnWidth(int column, bool isOriginal, CellsUnitType unitType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | The column index. |
| isOriginal | Boolean | Indicates whether getting original width. |
| unitType | CellsUnitType |  |

### See Also

* enum [CellsUnitType](../../cellsunittype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetColumnWidth(int) {#getcolumnwidth}

Gets the width(in unit of characters) of the specified column in normal view

```csharp
public double GetColumnWidth(int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index |

### Return Value

Width of column. For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


