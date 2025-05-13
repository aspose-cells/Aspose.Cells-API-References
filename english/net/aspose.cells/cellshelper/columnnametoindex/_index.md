---
title: CellsHelper.ColumnNameToIndex
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper method. Gets column index according to column name
type: docs
url: /net/aspose.cells/cellshelper/columnnametoindex/
---
## CellsHelper.ColumnNameToIndex method

Gets column index according to column name.

```csharp
public static int ColumnNameToIndex(string columnName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnName | String | Column name. |

### Return Value

Column index.

### Examples

```csharp
// Called: int columnIndex = CellsHelper.ColumnNameToIndex("BAA");
public void CellsHelper_Method_ColumnNameToIndex()
{
    int columnIndex = CellsHelper.ColumnNameToIndex("BAA");
    Assert.AreEqual(CellsHelper.ColumnIndexToName(columnIndex), "BAA");
}
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


