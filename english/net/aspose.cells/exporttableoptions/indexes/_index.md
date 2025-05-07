---
title: ExportTableOptions.Indexes
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions property. The indexes of columns/rows which should be exported out
type: docs
url: /net/aspose.cells/exporttableoptions/indexes/
---
## ExportTableOptions.Indexes property

The indexes of columns/rows which should be exported out.

```csharp
public int[] Indexes { get; set; }
```

### Examples

```csharp
// Called: options.Indexes = new int[] { 0, 2 };
[Test]
        public void Property_Indexes()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Test_164241.xls");
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


