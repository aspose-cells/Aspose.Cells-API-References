---
title: AutoFilter.Sorter
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter property. Gets the data sorter
type: docs
url: /net/aspose.cells/autofilter/sorter/
---
## AutoFilter.Sorter property

Gets the data sorter.

```csharp
public DataSorter Sorter { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(SortOrder.Descending, table.AutoFilter.Sorter.Keys[0].Order);
[Test]
        public void Property_Sorter()
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

* class [DataSorter](../../datasorter/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


