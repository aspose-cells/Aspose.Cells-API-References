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
// Called: opts.Indexes = new int[] { 5, 3, 2, 0 };
public void ExportTableOptions_Property_Indexes()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    //Access first worksheet 
    Worksheet ws = workbook.Worksheets[0];

    //Specify export table options - explains the usage of Indexes property 
    ExportTableOptions opts = new ExportTableOptions();
    opts.ExportColumnName = true;
    opts.Indexes = new int[] { 5, 3, 2, 0 };

    //Export Data Table with Export Table Options 
    DataTable dt = ws.Cells.ExportDataTable(0, 0, 15, 6, opts);
}
```

### See Also

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


