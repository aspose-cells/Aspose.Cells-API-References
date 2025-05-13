---
title: ListObject.EndColumn
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets the end column of the range
type: docs
url: /net/aspose.cells.tables/listobject/endcolumn/
---
## ListObject.EndColumn property

Gets the end column of the range.

```csharp
public int EndColumn { get; }
```

### Examples

```csharp
// Called: table.Resize(table.StartRow, table.StartColumn, 43, table.EndColumn, table.ShowHeaderRow);
public void ListObject_Property_EndColumn()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    WorksheetCollection worksheets = workbook.Worksheets;
    Worksheet worksheet = worksheets["S.20.01.01"];

    Cells cells = worksheet.Cells;
    cells.CopyRows(cells, 8, 26, 18);

    ListObjectCollection listObjects = worksheet.ListObjects;
    ListObject table = listObjects["ClaimsPerPeriod"];
    table.Resize(table.StartRow, table.StartColumn, 43, table.EndColumn, table.ShowHeaderRow);
    workbook.Save(Constants.destPath + "example.xlsx");
    Style style = cells["E29"].GetStyle();
    AssertHelper.AreEqual(style.ForegroundColor, System.Drawing.Color.FromArgb(253, 234, 218));// System.Drawing.Color.FromArgb(253, 233, 217));
    style = cells["E43"].GetStyle();
   AssertHelper.AreEqual(style.ForegroundColor, System.Drawing.Color.FromArgb(217, 217, 217));
        

}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


