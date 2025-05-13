---
title: ExportTableOptions.DataTable
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions property. Gets and sets the DataTable which columns data type is assigned
type: docs
url: /net/aspose.cells/exporttableoptions/datatable/
---
## ExportTableOptions.DataTable property

Gets and sets the DataTable which columns' data type is assigned.

```csharp
public DataTable DataTable { get; set; }
```

### Examples

```csharp
// Called: options.DataTable = dt;
public void ExportTableOptions_Property_DataTable()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Cells cells = workbook.Worksheets[0].Cells;
    DataTable dt = new DataTable();
    dt.Columns.Add("a1", typeof(double));
    dt.Columns.Add("a2", typeof(string));
    ExportTableOptions options = new ExportTableOptions();
    options.ExportColumnName = true;
    options.Indexes = new int[] { 0, 2 };
    options.DataTable = dt;
   // cells.ExportDataTable(dt, 0, new int[] { 0, 2 }, 3, true);
    cells.ExportDataTable(0, 0, 3, 3, options);

}
```

### See Also

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


