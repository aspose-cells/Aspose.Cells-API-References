---
title: ProtectedRangeCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ProtectedRangeCollection property. Gets the ProtectedRange element at the specified index
type: docs
url: /net/aspose.cells/protectedrangecollection/item/
---
## ProtectedRangeCollection indexer

Gets the [`ProtectedRange`](../../protectedrange/) element at the specified index.

```csharp
public ProtectedRange this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: ProtectedRange r = workbook.Worksheets[0].AllowEditRanges[0];
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet51922.xlsx&quot;);
            ProtectedRange r = workbook.Worksheets[0].AllowEditRanges[0];
            Assert.IsTrue(r.IsProtectedWithPassword);
            workbook.Save(Constants.destPath + &quot;CellsNet51922.xlsb&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet51922.xlsb&quot;);
            Assert.IsTrue(r.IsProtectedWithPassword);

        }
```

### See Also

* class [ProtectedRange](../../protectedrange/)
* class [ProtectedRangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


