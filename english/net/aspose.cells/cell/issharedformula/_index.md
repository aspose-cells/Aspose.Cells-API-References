---
title: Cell.IsSharedFormula
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Indicates whether the cell formula is part of shared formula
type: docs
url: /net/aspose.cells/cell/issharedformula/
---
## Cell.IsSharedFormula property

Indicates whether the cell formula is part of shared formula.

```csharp
public bool IsSharedFormula { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(cell.IsSharedFormula);
[Test]
        public void Property_IsSharedFormula()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet58028.xlsx&quot;);
            ApplyFormulas(workbook, workbook.Worksheets[2]);
            Cell cell = workbook.Worksheets[2].Cells[&quot;D3&quot;];
            Assert.IsFalse(cell.IsSharedFormula);
            workbook.Save(Constants.destPath + &quot;CellsNet58028.xlsx&quot;);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


