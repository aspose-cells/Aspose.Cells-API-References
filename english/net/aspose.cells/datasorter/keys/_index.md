---
title: DataSorter.Keys
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. Gets the key list of data sorter
type: docs
url: /net/aspose.cells/datasorter/keys/
---
## DataSorter.Keys property

Gets the key list of data sorter.

```csharp
public DataSorterKeyCollection Keys { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(SortOrder.Descending, table.AutoFilter.Sorter.Keys[0].Order);
[Test]
        public void Property_Keys()
        {
            Workbook sourceWb = new Workbook(Constants.sourcePath + "CellsNet53104.xlsx");
            Workbook destWb = new Workbook();
            destWb.Copy(sourceWb);
            ListObject table = destWb.Worksheets[0].ListObjects[0];
            Assert.AreEqual(SortOrder.Descending, table.AutoFilter.Sorter.Keys[0].Order);
            destWb.Save(Constants.destPath + "CellsNet53104.xlsx");
        }
```

### See Also

* class [DataSorterKeyCollection](../../datasorterkeycollection/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


