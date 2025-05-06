---
title: Cells.IsColumnHidden
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Checks whether a column at given index is hidden
type: docs
url: /net/aspose.cells/cells/iscolumnhidden/
---
## Cells.IsColumnHidden method

Checks whether a column at given index is hidden.

```csharp
public bool IsColumnHidden(int columnIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | column index |

### Return Value

true if the column is hidden.

### Examples

```csharp
// Called: Assert.IsFalse(cells.IsColumnHidden(2));
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet45639.xml&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            Assert.IsTrue(cells.IsColumnHidden(1));
            Assert.IsFalse(cells.IsColumnHidden(0));
            Assert.IsFalse(cells.IsColumnHidden(2));
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


