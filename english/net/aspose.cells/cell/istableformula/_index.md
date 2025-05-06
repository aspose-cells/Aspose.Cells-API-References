---
title: Cell.IsTableFormula
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Indicates whether this cell is part of table formula
type: docs
url: /net/aspose.cells/cell/istableformula/
---
## Cell.IsTableFormula property

Indicates whether this cell is part of table formula.

```csharp
public bool IsTableFormula { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(cells[&amp;quot;R53&amp;quot;].IsTableFormula);
[Test]
        public void Property_IsTableFormula()
        {
            Workbook workbook = new Workbook(Constants.batchPath + @&quot;calculate\CELLSNET_12475TableFormula.xls&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            Assert.IsTrue(cells[&quot;R53&quot;].IsTableFormula);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


