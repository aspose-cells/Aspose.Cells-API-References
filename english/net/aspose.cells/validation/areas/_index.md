---
title: Validation.Areas
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Gets all CellArea which contain the data validation settings
type: docs
url: /net/aspose.cells/validation/areas/
---
## Validation.Areas property

Gets all [`CellArea`](../../cellarea/) which contain the data validation settings.

```csharp
public CellArea[] Areas { get; }
```

### Examples

```csharp
// Called: CellArea cellarea = (CellArea)validation.Areas[i];
private void Property_Areas(Workbook workbook, CellArea cellarea1, CellArea cellarea2, CellArea cellarea3)
        {
            Worksheet sheet = workbook.Worksheets[0];
            testAreEqual(1, sheet.Validations.Count, caseName);
            Validation validation = sheet.Validations[0];
            testAreEqual(3, validation.Areas.Length, caseName);
            for (int i = 0; i < validation.Areas.Length; i++)
            {
                CellArea cellarea = (CellArea)validation.Areas[i];
                 if (cellarea.StartRow == cellarea1.StartRow)
                {
                    AssertHelper.checkCellArea(cellarea1, cellarea);
                }
                else if (cellarea.StartRow == cellarea2.StartRow)
                {
                    AssertHelper.checkCellArea(cellarea2, cellarea);
                }
                else if (cellarea.StartRow == cellarea3.StartRow)
                {
                    AssertHelper.checkCellArea(cellarea3, cellarea);
                }
            }
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


