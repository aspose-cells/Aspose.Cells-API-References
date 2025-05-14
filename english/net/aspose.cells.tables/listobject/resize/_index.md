---
title: ListObject.Resize
second_title: Aspose.Cells for .NET API Reference
description: ListObject method. Resize the range of the list object
type: docs
url: /net/aspose.cells.tables/listobject/resize/
---
## ListObject.Resize method

Resize the range of the list object.

```csharp
public void Resize(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The start row index of the new range. |
| startColumn | Int32 | The start column index of the new range. |
| endRow | Int32 | The end row index of the new range. |
| endColumn | Int32 | The end column index of the new range. |
| hasHeaders | Boolean | Whether this table has headers. |

### Examples

```csharp
// Called: selectedTable.Resize(1, 1, 9, 2, true);
public void ListObject_Method_Resize()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet selectedSheet = workbook.Worksheets["Rules"];

    var selectedTable = selectedSheet.ListObjects["tab_commercial_role_list"];
    selectedTable.Resize(1, 1, 9, 2, true);
    Cell b9 = selectedSheet.Cells["B9"];
    Style style = b9.GetStyle();
    Assert.AreEqual(style.Borders[BorderType.LeftBorder].LineStyle, CellBorderType.Thin);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


