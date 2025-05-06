---
title: ValidationCollection.RemoveACell
second_title: Aspose.Cells for .NET API Reference
description: ValidationCollection method. Removes all validation setting on the cell
type: docs
url: /net/aspose.cells/validationcollection/removeacell/
---
## ValidationCollection.RemoveACell method

Removes all validation setting on the cell.

```csharp
public void RemoveACell(int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index of the cell. |
| column | Int32 | The column index of the cell. |

### Examples

```csharp
// Called: cell.Worksheet.Validations.RemoveACell(cell.Row, cell.Column);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];
            var cell = ws.Cells[0, 0];
            ValidationCollection validations = ws.Validations;
            CellArea cellArea = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 0,
                EndColumn = 0
            };

            Validation validation = validations[validations.Add(cellArea)];
            validation.Type = ValidationType.List;
            validation.Formula1 = null;

            cell.Worksheet.Validations.RemoveACell(cell.Row, cell.Column);
            Assert.AreEqual(0, cell.Worksheet.Validations.Count);
            workbook.Save(Constants.destPath + &quot;CellsNet47374.xlsx&quot;);
        }
```

### See Also

* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


