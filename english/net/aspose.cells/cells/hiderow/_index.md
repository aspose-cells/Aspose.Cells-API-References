---
title: Cells.HideRow
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Hides a row
type: docs
url: /net/aspose.cells/cells/hiderow/
---
## Cells.HideRow method

Hides a row.

```csharp
public void HideRow(int row)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |

### Examples

```csharp
// Called: cells.HideRow(0);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.SetRowHeight(0, 12.75);
            cells.HideRow(0);
            cells.UnhideRow(0, -1);
            Assert.AreEqual(cells.GetRowHeight(0), 12.75);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


