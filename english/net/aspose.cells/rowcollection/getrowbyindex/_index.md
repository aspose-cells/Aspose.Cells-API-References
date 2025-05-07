---
title: RowCollection.GetRowByIndex
second_title: Aspose.Cells for .NET API Reference
description: RowCollection method. Gets the row object by the position in the list
type: docs
url: /net/aspose.cells/rowcollection/getrowbyindex/
---
## RowCollection.GetRowByIndex method

Gets the row object by the position in the list.

```csharp
public Row GetRowByIndex(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The position. |

### Return Value

The Row object at given position.

### Examples

```csharp
// Called: Assert.IsTrue(sheet.Cells.Rows.GetRowByIndex(0) == null);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Assert.IsTrue(sheet.Cells.Rows.GetRowByIndex(0) == null);
            
        }
```

### See Also

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


