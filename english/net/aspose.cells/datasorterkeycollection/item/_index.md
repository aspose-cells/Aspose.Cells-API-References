---
title: DataSorterKeyCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: DataSorterKeyCollection property. Gets and sets DataSorterKey by index
type: docs
url: /net/aspose.cells/datasorterkeycollection/item/
---
## DataSorterKeyCollection indexer

Gets and sets [`DataSorterKey`](../../datasorterkey/) by index.

```csharp
public DataSorterKey this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Examples

```csharp
// Called: Assert.AreEqual(SortOrder.Descending, table.AutoFilter.Sorter.Keys[0].Order);
[Test]
        public void Property_Int32_()
        {
            Workbook sourceWb = new Workbook(Constants.sourcePath + &quot;CellsNet53104.xlsx&quot;);
            Workbook destWb = new Workbook();
            destWb.Copy(sourceWb);
            ListObject table = destWb.Worksheets[0].ListObjects[0];
            Assert.AreEqual(SortOrder.Descending, table.AutoFilter.Sorter.Keys[0].Order);
            destWb.Save(Constants.destPath + &quot;CellsNet53104.xlsx&quot;);
        }
```

### See Also

* class [DataSorterKey](../../datasorterkey/)
* class [DataSorterKeyCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


