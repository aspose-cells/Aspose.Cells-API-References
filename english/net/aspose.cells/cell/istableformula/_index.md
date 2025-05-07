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
// Called: Assert.AreEqual(true, wb.Worksheets[0].Cells["D5"].IsTableFormula, "D5.IsTableFormula after open");
[Test]
        public void Property_IsTableFormula()
        {
            Workbook wb = new Workbook(Constants.sourcePath +"Formula/CellsNet40997.xlsm");
            Assert.AreEqual(true, wb.Worksheets[0].Cells["D5"].IsTableFormula, "D5.IsTableFormula after open");
            wb = Util.ReSave(wb, SaveFormat.Xlsm);
            Assert.AreEqual(true, wb.Worksheets[0].Cells["D5"].IsTableFormula, "D5.IsTableFormula after resave and open");
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


