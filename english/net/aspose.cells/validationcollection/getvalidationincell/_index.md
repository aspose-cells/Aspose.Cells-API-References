---
title: ValidationCollection.GetValidationInCell
second_title: Aspose.Cells for .NET API Reference
description: ValidationCollection method. Gets the validation applied to given cell
type: docs
url: /net/aspose.cells/validationcollection/getvalidationincell/
---
## ValidationCollection.GetValidationInCell method

Gets the validation applied to given cell.

```csharp
public Validation GetValidationInCell(int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |

### Return Value

Returns a [`Validation`](../../validation/) object or null if there is no validation for given cell

### Examples

```csharp
// Called: var validator = worksheet.Validations.GetValidationInCell(row, col);
static void Method_Int32_(Worksheet worksheet, string[] cells)
        {
            foreach (string cell in cells)
            {
                int row = 0, col = 0;
                CellsHelper.CellNameToIndex(cell, out row, out col);

                var validator = worksheet.Validations.GetValidationInCell(row, col);

                var name = FindNameReference(worksheet.Workbook.Worksheets.Names, validator.Formula1);

                Aspose.Cells.Range range = name.GetRange(worksheet.Index, row, col);

                Assert.AreEqual(range != null, true);
            }

        }
```

### See Also

* class [Validation](../../validation/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


