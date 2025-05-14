---
title: ExportTableOptions.PlotVisibleCells
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions property. Only exports visible cells
type: docs
url: /net/aspose.cells/exporttableoptions/plotvisiblecells/
---
## ExportTableOptions.PlotVisibleCells property

Only exports visible cells.

```csharp
public bool PlotVisibleCells { get; set; }
```

### Examples

```csharp
// Called: PlotVisibleCells = true,
public void ExportTableOptions_Property_PlotVisibleCells()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    // Access the first worksheet
    Worksheet worksheet = workbook.Worksheets[0];

    // Specify export table options
    ExportTableOptions exportOptions = new ExportTableOptions()
    {
        PlotVisibleCells = true,
        PlotVisibleColumns = true,
        PlotVisibleRows = true
    };

    // Export the data from worksheet with export options
    DataTable dataTable = worksheet.Cells.ExportDataTable(1, 0, 5, 7, exportOptions);
    Assert.AreEqual(1, dataTable.Rows.Count);

}
```

### See Also

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


