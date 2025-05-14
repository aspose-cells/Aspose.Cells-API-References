---
title: DataSorter.HasHeaders
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. Represents whether the range has headers
type: docs
url: /net/aspose.cells/datasorter/hasheaders/
---
## DataSorter.HasHeaders property

Represents whether the range has headers.

```csharp
public bool HasHeaders { get; set; }
```

### Examples

```csharp
// Called: sorter.HasHeaders = true;
public void DataSorter_Property_HasHeaders()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "Sort/File_for_CustomSort_ASPOSE_Forum_Question.xlsx");
    DataSorter sorter = workbook.DataSorter;
    sorter.AddKey(0, SortOrder.Ascending, "aaa,ddd,ccc,bbb");
    sorter.HasHeaders = true;
    sorter.Sort(workbook.Worksheets[1].Cells, CellArea.CreateCellArea("A1", "C23"));
    Cells cells = workbook.Worksheets[1].Cells;
    Assert.AreEqual(cells["A2"].StringValue, "aaa");
    Assert.AreEqual(cells["A7"].StringValue, "ddd");
    Assert.AreEqual(cells["A12"].StringValue, "ccc");
    Assert.AreEqual(cells["A18"].StringValue, "bbb");
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


