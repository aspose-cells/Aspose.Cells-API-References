---
title: ExportTableOptions.ExportColumnName
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions property. Indicates whether the data in the first row are exported to the column name of the DataTable. The default value is false
type: docs
url: /net/aspose.cells/exporttableoptions/exportcolumnname/
---
## ExportTableOptions.ExportColumnName property

Indicates whether the data in the first row are exported to the column name of the DataTable. The default value is false.

```csharp
public bool ExportColumnName { get; set; }
```

### Examples

```csharp
// Called: options.ExportColumnName = true;
public void ExportTableOptions_Property_ExportColumnName()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Cells cells = workbook.Worksheets[0].Cells;
    DataTable dt = new DataTable();
    dt.Columns.Add("a1", typeof(double));
    dt.Columns.Add("a2", typeof(string));
    ExportTableOptions options = new ExportTableOptions();
    options.ExportColumnName = true;
    options.IsVertical = true;
    options.Indexes = new int[] { 0, 2 };
    options.DataTable = dt;
    // cells.ExportDataTable(dt, 0, new int[] { 0, 2 }, 3, true);
    cells.ExportDataTable(0, 0, 2, 3, options);


}
```

### See Also

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


