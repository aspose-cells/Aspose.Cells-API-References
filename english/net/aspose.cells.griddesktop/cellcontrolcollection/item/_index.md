---
title: Item
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 10
url: /net/aspose.cells.griddesktop/cellcontrolcollection/item/
---
## CellControlCollection indexer (1 of 2)

Gets the cell control at specified row and column index.

```csharp
public CellControl this[int row, int col] { get; }
```

| Parameter | Description |
| --- | --- |
| row | row index. |
| col | column index. |

### Remarks

If there is not a CellControl object at specified row column index, this will check the column CellControl object.

### See Also

* class [CellControl](../../cellcontrol)
* class [CellControlCollection](../../cellcontrolcollection)
* namespace [Aspose.Cells.GridDesktop](../../cellcontrolcollection)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## CellControlCollection indexer (2 of 2)

Gets the cell control by specified cell name.

```csharp
public CellControl this[string cellName] { get; }
```

| Parameter | Description |
| --- | --- |
| cellName | cell name(in excel name format, like 'A1', 'F22') |

### Remarks

If there is not a CellControl object at specified row column index, this will check the column CellControl object.

### See Also

* class [CellControl](../../cellcontrol)
* class [CellControlCollection](../../cellcontrolcollection)
* namespace [Aspose.Cells.GridDesktop](../../cellcontrolcollection)
* assembly [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->