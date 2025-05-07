---
title: ExportTableOptions.IsVertical
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions property. True if a row in Workbook file represents a row in DataTable. False if a column in Workbook file represents a row in DataTable
type: docs
url: /net/aspose.cells/exporttableoptions/isvertical/
---
## ExportTableOptions.IsVertical property

True if a row in Workbook file represents a row in DataTable. False if a column in Workbook file represents a row in DataTable.

```csharp
public bool IsVertical { get; set; }
```

### Examples

```csharp
// Called: options.IsVertical = true;
[Test]
        public void Property_IsVertical()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Test_180922.xls");
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


