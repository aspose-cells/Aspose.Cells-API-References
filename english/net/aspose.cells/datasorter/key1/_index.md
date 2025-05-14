---
title: DataSorter.Key1
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. Represents first sorted column indexabsolute position column A is 0 B is 1 
type: docs
url: /net/aspose.cells/datasorter/key1/
---
## DataSorter.Key1 property

Represents first sorted column index(absolute position, column A is 0, B is 1, ...).

```csharp
public int Key1 { get; set; }
```

### Examples

```csharp
// Called: dataSorter.Key1 = column;
private static void DataSorter_Property_Key1(DataSorter dataSorter, Cells cells, int column, SortOrder sortOrder, int startRow, int endRow)
        {
            CellArea sortArea = new CellArea();
            sortArea.StartRow = startRow;
            sortArea.EndRow = endRow;
            sortArea.StartColumn = 0;
            sortArea.EndColumn = cells.MaxDataColumn;
            dataSorter.Key1 = column;
            dataSorter.Order1 = sortOrder;
            dataSorter.Sort(cells, sortArea);
        }
```

### See Also

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


