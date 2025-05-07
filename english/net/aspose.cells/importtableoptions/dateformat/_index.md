---
title: ImportTableOptions.DateFormat
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Gets or sets date format string for cells with imported datetime values
type: docs
url: /net/aspose.cells/importtableoptions/dateformat/
---
## ImportTableOptions.DateFormat property

Gets or sets date format string for cells with imported datetime values.

```csharp
public string DateFormat { get; set; }
```

### Examples

```csharp
// Called: DateFormat = "YYYY-MM-DD"
private void Property_DateFormat(Workbook workbook, Aspose.Cells.Range range, DataTable tbl)
        {
            range.Worksheet.Cells.ImportData(tbl, range.FirstRow, range.FirstColumn,
                new ImportTableOptions()
                {
                    IsFieldNameShown = true,
                    InsertRows = true,
                    ConvertNumericData = false,
                    TotalRows = tbl.Rows.Count,
                    TotalColumns = tbl.Columns.Count,
                    DateFormat = "YYYY-MM-DD"
                });
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


