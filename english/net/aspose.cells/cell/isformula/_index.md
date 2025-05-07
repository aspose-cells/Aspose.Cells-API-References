---
title: Cell.IsFormula
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Represents if the specified cell contains formula
type: docs
url: /net/aspose.cells/cell/isformula/
---
## Cell.IsFormula property

Represents if the specified cell contains formula.

```csharp
public bool IsFormula { get; }
```

### Examples

```csharp
// Called: testAreEqual(false, cells[row, col].IsFormula, caseName);
private void Property_IsFormula(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            testAreEqual(0, cells[8, 0].IntValue, caseName);
            testAreEqual(0, cells[9, 0].IntValue, caseName);
            testAreEqual(6, cells[10, 0].IntValue, caseName);
            testAreEqual(0, cells[8, 1].IntValue, caseName);
            testAreEqual(0, cells[9, 1].IntValue, caseName);
            testAreEqual(6, cells[10, 1].IntValue, caseName);
            testAreEqual(1, cells[8, 2].IntValue, caseName);
            testAreEqual(0, cells[9, 2].IntValue, caseName);
            testAreEqual(6, cells[10, 2].IntValue, caseName);
            testAreEqual(6, cells[8, 3].IntValue, caseName);
            testAreEqual(0, cells[9, 3].IntValue, caseName);
            testAreEqual(6, cells[10, 3].IntValue, caseName);
            for (int row = 8; row <= 10; row++)
            {
                for (int col = 0; col <= 3; col++)
                {
                    testAreEqual(false, cells[row, col].IsFormula, caseName);
                }
            }
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


