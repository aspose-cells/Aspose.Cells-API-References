---
title: ImportTableOptions.ShiftFirstRowDown
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Indicates whether shifting the first row down when inserting rows
type: docs
url: /net/aspose.cells/importtableoptions/shiftfirstrowdown/
---
## ImportTableOptions.ShiftFirstRowDown property

Indicates whether shifting the first row down when inserting rows.

```csharp
public bool ShiftFirstRowDown { get; set; }
```

### Examples

```csharp
// Called: ShiftFirstRowDown = false,
public void ImportTableOptions_Property_ShiftFirstRowDown()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Cells cells = wb.Worksheets[0].Cells;
    DataTable table = new DataTable();
    table.Columns.Add(new DataColumn());
    table.Columns.Add(new DataColumn());
    table.Rows.Add("A", "");
    table.Rows.Add(null, null);
    table.Rows.Add("A", "A");

    var importTableOptions = new ImportTableOptions
    {
        IsFieldNameShown = false,
        ShiftFirstRowDown = false,
        InsertRows = true,
    };
    cells.ImportData(table, 3, 0, importTableOptions);
    Assert.AreEqual("=IF(AND(A3<>\"X\",A4=B4),\"Yes\",\"no\")", cells[3, 3].Formula, "D4.Formula");
}
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


