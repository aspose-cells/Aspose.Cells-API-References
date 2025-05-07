---
title: Cells.GetCell
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the Cell element or null at the specified cell row index and column index
type: docs
url: /net/aspose.cells/cells/getcell/
---
## Cells.GetCell method

Gets the [`Cell`](../../cell/) element or null at the specified cell row index and column index.

```csharp
[Obsolete("Use Cells.CheckCell(int row, int column) instead.")]
public Cell GetCell(int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index |
| column | Int32 | Column index |

### Return Value

Return Cell object if a Cell object exists. Return null if the cell does not exist.

### Remarks

NOTE: This member is now obsolete. Instead, please use CheckCell(int row, int column) method. This method will be removed 12 months later since February 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: var cell = workbook.Worksheets[0].Cells.GetCell(1,2);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            var cell = workbook.Worksheets[0].Cells.GetCell(1,2);
            cell.Worksheet.Validations[0].RemoveACell(cell.Row, cell.Column);
        }
```

### See Also

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


