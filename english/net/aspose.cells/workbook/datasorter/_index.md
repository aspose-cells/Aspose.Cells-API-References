---
title: Workbook.DataSorter
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets a DataSorter object to sort data
type: docs
url: /net/aspose.cells/workbook/datasorter/
---
## Workbook.DataSorter property

Gets a DataSorter object to sort data.

```csharp
public DataSorter DataSorter { get; }
```

### Examples

```csharp
// Called: DataSorter sorter = workbook.DataSorter;
[Test]
        public void Property_DataSorter()
        {
            //CELLSNET-57170
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSCPP1130.xlsx&quot;);
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;
            sorter.AddColorKey(0, SortOnType.CellColor, SortOrder.Ascending, Color.Red);
            sorter.Sort(workbook.Worksheets[0].Cells, CellArea.CreateCellArea(0, 0, 4, 3));
            Assert.AreEqual(5, workbook.Worksheets[0].Cells[&quot;A2&quot;].IntValue);
        }
```

### See Also

* class [DataSorter](../../datasorter/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


