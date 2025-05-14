---
title: Worksheet.Validations
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the data validation setting collection in the worksheet
type: docs
url: /net/aspose.cells/worksheet/validations/
---
## Worksheet.Validations property

Gets the data validation setting collection in the worksheet.

```csharp
public ValidationCollection Validations { get; }
```

### Examples

```csharp
// Called: var validator = worksheet.Validations.GetValidationInCell(row, col);
static void Worksheet_Property_Validations(Worksheet worksheet, string[] cells)
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

* class [ValidationCollection](../../validationcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


