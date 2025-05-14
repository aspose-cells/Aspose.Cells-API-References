---
title: Cells.HideRow
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Hides a row
type: docs
url: /net/aspose.cells/cells/hiderow/
---
## Cells.HideRow method

Hides a row.

```csharp
public void HideRow(int row)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |

### Examples

```csharp
// Called: excelDocument.Worksheets["CSC T"].Cells.HideRow(19);
public void Cells_Method_HideRow()
{
    Workbook excelDocument = new Workbook(Constants.sourcePath + "example.xlsx");
     
    excelDocument.Worksheets["CSC T"].Cells.HideRow(19);
    Assert.IsFalse(excelDocument.Worksheets["CSC T"].Cells.Rows[19].IsHeightMatched);
    excelDocument.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


