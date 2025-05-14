---
title: ValidationCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ValidationCollection property. Gets the Validation element at the specified index
type: docs
url: /net/aspose.cells/validationcollection/item/
---
## ValidationCollection indexer

Gets the [`Validation`](../../validation/) element at the specified index.

```csharp
public Validation this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Validation validation = sheet.Validations[0];
private void ValidationCollection_Property_Item(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            testAreEqual(1, sheet.Validations.Count, caseName);
            Validation validation = sheet.Validations[0];
            testAreEqual(2, validation.Areas.Length, caseName);
            bool IsSame = false;
            for (int i = 0; i < validation.Areas.Length; i++)
            {
                CellArea cellarea = (CellArea)validation.Areas[i];
                if (cellarea.StartRow == 1)
                {
                    AssertHelper.checkCellArea(1, 1, 4, 3, cellarea);
                    IsSame = true;
                }
                else if (cellarea.StartRow == 6)
                {
                    AssertHelper.checkCellArea(6, 1, 6, 3, cellarea);
                    IsSame = true;
                }
            }
            if (!IsSame)
            {
                AssertHelper.Fail("Validation object is not same");
            }
        }
```

### See Also

* class [Validation](../../validation/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


