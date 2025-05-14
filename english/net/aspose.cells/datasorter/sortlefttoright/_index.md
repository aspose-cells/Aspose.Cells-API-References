---
title: DataSorter.SortLeftToRight
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false
type: docs
url: /net/aspose.cells/datasorter/sortlefttoright/
---
## DataSorter.SortLeftToRight property

True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false.

```csharp
public bool SortLeftToRight { get; set; }
```

### Examples

```csharp
// Called: dataSorter.SortLeftToRight = true;
public void DataSorter_Property_SortLeftToRight()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    DataSorter dataSorter = workbook.DataSorter;

    dataSorter.Key1 = 0;
    CellArea area = new CellArea();
    area.StartRow = 0;
    area.EndRow = 4;
    area.StartColumn = 0;
    area.EndColumn = 2;
    dataSorter.SortLeftToRight = true;
    dataSorter.Sort(workbook.Worksheets[0].Cells, area);
    Assert.AreEqual(workbook.Worksheets[0].Cells["A1"].DoubleValue, 4);
    workbook.Save(Constants.destPath + "example.xls");

}
```

### See Also

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


