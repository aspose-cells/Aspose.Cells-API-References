---
title: CellsHelper.ColumnIndexToName
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper method. Gets column name according to column index
type: docs
url: /net/aspose.cells/cellshelper/columnindextoname/
---
## CellsHelper.ColumnIndexToName method

Gets column name according to column index.

```csharp
public static string ColumnIndexToName(int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |

### Return Value

Name of column.

### Examples

```csharp
// Called: + CellsHelper.ColumnIndexToName(cs[j]-shiftCol) + (i + 1 - shiftRow));
private void CellsHelper_Method_ColumnIndexToName(Cells cells, int shiftRow, int shiftCol, int[][] cols, object[][] vals)
        {
            for (int i = 0; i < cols.Length; i++)
            {
                if (cols[i] != null)
                {
                    int[] cs = cols[i];
                    object[] vs = vals[i];
                    for (int j = 0; j < cs.Length; j++)
                    {
                        Assert.AreEqual(vs[j], cells[i-shiftRow, cs[j]-shiftCol].Value,
                            CellsHelper.ColumnIndexToName(cs[j]) + (i + 1) + "->"
                            + CellsHelper.ColumnIndexToName(cs[j]-shiftCol) + (i + 1 - shiftRow));
                    }
                }
            }
        }
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


