---
title: ImportTableOptions.ConvertNumericData
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Gets or sets a value that indicates whether the string value should be converted to numeric or date value
type: docs
url: /net/aspose.cells/importtableoptions/convertnumericdata/
---
## ImportTableOptions.ConvertNumericData property

Gets or sets a value that indicates whether the string value should be converted to numeric or date value.

```csharp
public bool ConvertNumericData { get; set; }
```

### Examples

```csharp
// Called: options.ConvertNumericData = false;
private static void Property_ConvertNumericData(Workbook workbook, Aspose.Cells.Range range, DataTable tbl)
        {
            ImportTableOptions options = new ImportTableOptions();
            options.InsertRows = true;
            options.IsFieldNameShown = true;
            options.DateFormat = "YYYY-MM-DD";
            options.ConvertNumericData = false;
            options.ShiftFirstRowDown = false;
            range.Worksheet.Cells.ImportData(tbl, range.FirstRow, range.FirstColumn, options);
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


