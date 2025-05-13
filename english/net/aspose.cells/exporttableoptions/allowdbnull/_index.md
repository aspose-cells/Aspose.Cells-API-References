---
title: ExportTableOptions.AllowDBNull
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions property. This value indicates whether DBNulls are allowed in this table
type: docs
url: /net/aspose.cells/exporttableoptions/allowdbnull/
---
## ExportTableOptions.AllowDBNull property

This value indicates whether DBNulls are allowed in this table.

```csharp
public bool AllowDBNull { get; set; }
```

### Examples

```csharp
// Called: AllowDBNull = false
public void ExportTableOptions_Property_AllowDBNull()
{
    string filePath = Constants.sourcePath + "example.xls";
    Workbook excel = new Workbook(filePath);
    Worksheet sheet = excel.Worksheets[0];
    int maxRow = sheet.Cells.MaxDataRow + 1;
    int maxCol = sheet.Cells.MaxDataColumn + 1;

    var opts = new ExportTableOptions
    {
        CheckMixedValueType = true,
        ExportColumnName = true,
        AllowDBNull = false

    };
    DataTable table = sheet.Cells.ExportDataTable(0, 0, maxRow, maxCol, opts);
    int errors = CheckColTypes(table);

    // Test new Excel (xlsx).
    filePath = Constants.sourcePath + "example.xlsx";

    excel = new Workbook(filePath);
    sheet = excel.Worksheets[0];
    maxRow = sheet.Cells.MaxDataRow + 1;
    maxCol = sheet.Cells.MaxDataColumn + 1;

    opts = new ExportTableOptions
    {
        CheckMixedValueType = true,
        ExportColumnName = true,
        AllowDBNull = false
    };
    table = sheet.Cells.ExportDataTable(0, 0, maxRow, maxCol, opts);
    errors += CheckColTypes(table);

    Assert.AreEqual(0, errors);
}
```

### See Also

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


