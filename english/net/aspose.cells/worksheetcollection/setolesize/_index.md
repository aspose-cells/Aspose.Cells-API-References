---
title: WorksheetCollection.SetOleSize
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Sets displayed size when Workbook file is used as an Ole object
type: docs
url: /net/aspose.cells/worksheetcollection/setolesize/
---
## WorksheetCollection.SetOleSize method

Sets displayed size when Workbook file is used as an Ole object.

```csharp
public void SetOleSize(int startRow, int endRow, int startColumn, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index. |
| endRow | Int32 | End row index. |
| startColumn | Int32 | Start column index. |
| endColumn | Int32 | End column index. |

### Remarks

This method is generally used to adjust display size in ppt file or doc file.

### Examples

```csharp
// Called: workbook.Worksheets.SetOleSize(0, 10, 0, 10);
public void WorksheetCollection_Method_SetOleSize()
{
    Workbook workbook = new Workbook();
    workbook.Worksheets.SetOleSize(0, 10, 0, 10);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(((CellArea)workbook.Worksheets.OleSize).EndRow, 10);
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    Assert.AreEqual(((CellArea)workbook.Worksheets.OleSize).EndRow, 10);

}
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


