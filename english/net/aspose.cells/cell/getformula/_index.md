---
title: Cell.GetFormula
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Get the formula of this cell
type: docs
url: /net/aspose.cells/cell/getformula/
---
## Cell.GetFormula method

Get the formula of this cell.

```csharp
public string GetFormula(bool isR1C1, bool isLocal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |

### Return Value

the formula of this cell.

### Examples

```csharp
// Called: Assert.AreEqual(fmlStd, cell.GetFormula(false, false), procInfo + &amp;quot;-GetFormula(local as false)&amp;quot;);
private void Method_Boolean_(string procInfo, Cell cell, string fmlStd, string fmlLoc)
	    {
            Assert.AreEqual(fmlStd, cell.Formula, procInfo + &quot;-Formula&quot;);
            Assert.AreEqual(fmlLoc, cell.FormulaLocal, procInfo + &quot;-FormulaLocal&quot;);
            Assert.AreEqual(fmlStd, cell.GetFormula(false, false), procInfo + &quot;-GetFormula(local as false)&quot;);
            Assert.AreEqual(fmlLoc, cell.GetFormula(false, true), procInfo + &quot;-GetFormula(local as true)&quot;);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


