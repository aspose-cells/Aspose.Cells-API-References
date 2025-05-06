---
title: Enum SortOrder
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.SortOrder enum. Represents sort order for the data range
type: docs
url: /net/aspose.cells/sortorder/
---
## SortOrder enumeration

Represents sort order for the data range.

```csharp
public enum SortOrder
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Ascending | `0` | Sorts data in ascending order |
| Descending | `1` | Sorts data in descending order |
| Natural | `2` | Keeps original data order without sorting. Only applies to some special scenarios such as PivotTable. |

### Examples

```csharp
// Called: ApplySort(workbook.DataSorter, cells, 3, SortOrder.Ascending, 2, 4);
[Test]
        public void Type_SortOrder()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Sort/CELLSNET17907.xls&quot;);
            Cells cells = workbook.Worksheets[0].Cells;

            ////case 1
            ApplySort(workbook.DataSorter, cells, 3, SortOrder.Ascending, 2, 4);

            ////case 2
            // workbook.Worksheets[0].Cells.UngroupRows(8, 10);
            ApplySort(workbook.DataSorter, cells, 3, SortOrder.Ascending, 8, 10);

            ////case 3
            ApplySort(workbook.DataSorter, cells, 3, SortOrder.Ascending, 15, 16);

            ////case 4
            ApplySort(workbook.DataSorter, cells, 3, SortOrder.Ascending, 25, 26);

            ////case 5
            ApplySort(workbook.DataSorter, cells, 3, SortOrder.Ascending, 32, 33);

            workbook.CalculateFormula();
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;D10&quot;].StringValue, &quot;Mixed&quot;);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


