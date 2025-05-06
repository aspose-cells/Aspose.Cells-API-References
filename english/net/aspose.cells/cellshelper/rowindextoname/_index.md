---
title: CellsHelper.RowIndexToName
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper method. Gets row name according to row index
type: docs
url: /net/aspose.cells/cellshelper/rowindextoname/
---
## CellsHelper.RowIndexToName method

Gets row name according to row index.

```csharp
public static string RowIndexToName(int row)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |

### Return Value

Name of row.

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;11&amp;quot;, CellsHelper.RowIndexToName(r));
[Test]
        public void Method_Int32_()
        {
            int r = 10;
            Assert.AreEqual(&quot;11&quot;, CellsHelper.RowIndexToName(r));
            Assert.AreEqual(r, CellsHelper.RowNameToIndex(&quot;11&quot;));
        }
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


