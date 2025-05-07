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
[Test]
        public void Property_HasHeaders()
        {
            //CELLSNET-57170
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSCPP1130.xlsx");
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;
            sorter.AddColorKey(0, SortOnType.CellColor, SortOrder.Ascending, Color.Red);
            sorter.Sort(workbook.Worksheets[0].Cells, CellArea.CreateCellArea(0, 0, 4, 3));
            Assert.AreEqual(5, workbook.Worksheets[0].Cells["A2"].IntValue);
        }
```

### See Also

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


