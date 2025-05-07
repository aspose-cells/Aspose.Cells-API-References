---
title: DataSorter.Order1
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. Represents sort order of the first key
type: docs
url: /net/aspose.cells/datasorter/order1/
---
## DataSorter.Order1 property

Represents sort order of the first key.

```csharp
public SortOrder Order1 { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(sorter.Order1, SortOrder.Descending); //Ascending
[Test]
        public void Property_Order1()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Templateexcel3Rowsplu+formula2.xlsx");
            ListObject listObject = workbook.Worksheets[0].ListObjects[0];
            listObject.AutoFilter.Refresh();
            DataSorter sorter = listObject.AutoFilter.Sorter;
           Assert.AreEqual(sorter.Order1, SortOrder.Descending); //Ascending

        }
```

### See Also

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


