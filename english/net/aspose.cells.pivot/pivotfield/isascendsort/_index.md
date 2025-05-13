---
title: PivotField.IsAscendSort
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether the specified PivotTable field is autosorted ascending
type: docs
url: /net/aspose.cells.pivot/pivotfield/isascendsort/
---
## PivotField.IsAscendSort property

Indicates whether the specified PivotTable field is autosorted ascending.

```csharp
public bool IsAscendSort { get; set; }
```

### Examples

```csharp
// Called: sortField.IsAscendSort = false;
public void PivotField_Property_IsAscendSort()
{
    string filePath = Constants.PivotTableSourcePath + @"JAVA43101_";

    Workbook workbook = new Workbook(filePath + "Unsorted pivot table - input.xlsx");
    Worksheet worksheet = workbook.Worksheets["PivotTable"];

    PivotTable tbl = worksheet.PivotTables[0];


    PivotField sortField = tbl.RowFields[1];
    sortField.IsAutoSort = true;
    sortField.IsAscendSort = false;
    sortField.AutoSortField = 2;

    tbl.RefreshData();
    tbl.CalculateData();

    workbook.Save(CreateFolder(filePath) + "out.xlsx");
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


