---
title: Cells.CheckRow
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the Row element or null at the specified cell row index
type: docs
url: /net/aspose.cells/cells/checkrow/
---
## Cells.CheckRow method

Gets the [`Row`](../../row/) element or null at the specified cell row index.

```csharp
public Row CheckRow(int row)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index |

### Return Value

Returns [`Row`](../../row/) object If the row object does exist, otherwise returns null.

### Examples

```csharp
// Called: Assert.IsNotNull(cells.CheckRow(2));
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells["B3"].PutValue("4");
            cells.Columns[4].IsHidden = true;
            Assert.IsNotNull(cells.CheckColumn(4));
            Assert.IsNotNull(cells.CheckRow(2));
        }
```

### See Also

* class [Row](../../row/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


