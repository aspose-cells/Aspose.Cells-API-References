---
title: ImportTableOptions.ImportTableOptions
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions constructor. Creates the default importing options
type: docs
url: /net/aspose.cells/importtableoptions/importtableoptions/
---
## ImportTableOptions constructor

Creates the default importing options.

```csharp
public ImportTableOptions()
```

### Examples

```csharp
// Called: ImportTableOptions options = new ImportTableOptions();
public void ImportTableOptions_Constructor()
{
    Workbook workbook = new Workbook();
    DataTable dt = new DataTable();
    dt.Columns.Add("C1");
    dt.Rows.Add("<b>aa</b>");
    Cells cells = workbook.Worksheets[0].Cells;
    ImportTableOptions options = new ImportTableOptions();
    options.IsHtmlString = true;
    options.IsFieldNameShown = true;
    cells.ImportData(dt, 0, 0, options);
    Assert.IsTrue(cells["A2"].GetStyle().Font.IsBold);
}
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


