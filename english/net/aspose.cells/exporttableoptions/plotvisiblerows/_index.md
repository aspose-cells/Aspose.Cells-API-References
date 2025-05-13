---
title: ExportTableOptions.PlotVisibleRows
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions property. Only exports visible rows
type: docs
url: /net/aspose.cells/exporttableoptions/plotvisiblerows/
---
## ExportTableOptions.PlotVisibleRows property

Only exports visible rows.

```csharp
public bool PlotVisibleRows { get; set; }
```

### Examples

```csharp
// Called: options.PlotVisibleRows = true;//CELLSNET-42399
public void ExportTableOptions_Property_PlotVisibleRows()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells["A1"].PutValue("Col1");
    cells["A2"].PutValue(2);
    DataTable dt = new DataTable();
    dt.Columns.Add("Col1",typeof(decimal));
    ExportTableOptions options = new ExportTableOptions();
    options.PlotVisibleRows = true;//CELLSNET-42399
    options.ExportColumnName = true;
    options.DataTable = dt;
    cells.ExportDataTable(0,0,2,1,options);

                
}
```

### See Also

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


