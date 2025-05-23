---
title: Validation.RemoveACell
second_title: Aspose.Cells for .NET API Reference
description: Validation method. Remove the validation settings in the cell
type: docs
url: /net/aspose.cells/validation/removeacell/
---
## Validation.RemoveACell method

Remove the validation settings in the cell.

```csharp
public void RemoveACell(int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |

### Examples

```csharp
// Called: cell.Worksheet.Validations[0].RemoveACell(cell.Row, cell.Column);
public void Validation_Method_RemoveACell()
{
    Workbook workbook = new Workbook();
    var cell = workbook.Worksheets[0].Cells.GetCell(1,2);
    cell.Worksheet.Validations[0].RemoveACell(cell.Row, cell.Column);
}
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


