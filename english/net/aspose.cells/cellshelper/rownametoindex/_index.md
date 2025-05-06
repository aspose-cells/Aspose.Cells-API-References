---
title: CellsHelper.RowNameToIndex
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper method. Gets row index according to row name
type: docs
url: /net/aspose.cells/cellshelper/rownametoindex/
---
## CellsHelper.RowNameToIndex method

Gets row index according to row name.

```csharp
public static int RowNameToIndex(string rowName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowName | String | Row name. |

### Return Value

Row index.

### Examples

```csharp
// Called: Assert.AreEqual(r, CellsHelper.RowNameToIndex(&amp;quot;11&amp;quot;));
[Test]
        public void Method_String_()
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


