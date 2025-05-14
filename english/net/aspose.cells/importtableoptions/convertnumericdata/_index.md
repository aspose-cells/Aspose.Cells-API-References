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
// Called: options.ConvertNumericData = true;
public void ImportTableOptions_Property_ConvertNumericData()
{
    Workbook workbook = new Workbook();
    DataTable dt = new DataTable();
    dt.Columns.Add("C1");
    dt.Rows.Add("<baa</b>");
    Cells cells = workbook.Worksheets[0].Cells;
    ImportTableOptions options = new ImportTableOptions();
    options.IsHtmlString = false;
    options.IsFieldNameShown = true;
    options.ConvertNumericData = true;
    cells.ImportData(dt, 0, 0, options);
    Assert.AreEqual("<baa</b>", cells["A2"].StringValue);
}
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


