---
title: Cell.FormulaLocal
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Get the locale formatted formula of the cell
type: docs
url: /net/aspose.cells/cell/formulalocal/
---
## Cell.FormulaLocal property

Get the locale formatted formula of the cell.

```csharp
public string FormulaLocal { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(fmlLoc, cell.FormulaLocal, procInfo + "-FormulaLocal");
private void Cell_Property_FormulaLocal(string procInfo, Cell cell, string fmlStd, string fmlLoc)
	    {
            Assert.AreEqual(fmlStd, cell.Formula, procInfo + "-Formula");
            Assert.AreEqual(fmlLoc, cell.FormulaLocal, procInfo + "-FormulaLocal");
            Assert.AreEqual(fmlStd, cell.GetFormula(false, false), procInfo + "-GetFormula(local as false)");
            Assert.AreEqual(fmlLoc, cell.GetFormula(false, true), procInfo + "-GetFormula(local as true)");
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


