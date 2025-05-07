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
[Test]
        public void Property_DataTable()
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


