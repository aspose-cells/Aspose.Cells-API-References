---
title: ExportTableOptions.CheckMixedValueType
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions property. False Aspose.Cells will set the DataColumns type by the value type of the first row for performance. True Aspose.Cells will check whether the value type in the column are mixed before set the DataColumns type And the value type are mixed the DataColumns type will be string
type: docs
url: /net/aspose.cells/exporttableoptions/checkmixedvaluetype/
---
## ExportTableOptions.CheckMixedValueType property

False, Aspose.Cells will set the DataColumn's type by the value type of the first row for performance. True, Aspose.Cells will check whether the value type in the column are mixed before set the DataColumn's type And the value type are mixed, the DataColumn's type will be string.

```csharp
public bool CheckMixedValueType { get; set; }
```

### Examples

```csharp
// Called: CheckMixedValueType = true,
public void ExportTableOptions_Property_CheckMixedValueType()
{
    Workbook excel = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet sheet = excel.Worksheets[0];
    int maxRow = sheet.Cells.MaxDataRow + 1;
    int maxCol = sheet.Cells.MaxDataColumn + 1;

    var opts = new ExportTableOptions
    {
        CheckMixedValueType = true,
        ExportColumnName = true,
        AllowDBNull = true
    };
    DataTable table = sheet.Cells.ExportDataTable(0, 0, maxRow, maxCol, opts);
    Assert.AreEqual(2, table.Columns.Count);
    Assert.AreEqual(5, table.Rows.Count);
    Assert.IsTrue(table.Columns.Contains("id"));
    Assert.AreEqual("System.Double", table.Columns["id"].DataType.FullName);
    Assert.IsTrue(table.Columns.Contains("value date"));
    Assert.AreEqual("System.DateTime", table.Columns["value date"].DataType.FullName);
}
```

### See Also

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


