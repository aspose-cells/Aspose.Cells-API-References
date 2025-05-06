---
title: PivotItem.GetFormula
second_title: Aspose.Cells for .NET API Reference
description: PivotItem method. Gets the formula of this calculated item. Only works when this item is calculated item
type: docs
url: /net/aspose.cells.pivot/pivotitem/getformula/
---
## PivotItem.GetFormula method

Gets the formula of this calculated item. Only works when this item is calculated item.

```csharp
public string GetFormula()
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;=&amp;apos;w&amp;apos;&amp;apos;e&amp;apos;&amp;quot;,wb.Worksheets[0].PivotTables[0].RowFields[0].PivotItems[2].GetFormula());
[Test]
        public void Method_GetFormula()
        {

            Workbook wb = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET56419.xlsx&quot;);
           Assert.AreEqual(&quot;=&apos;b&apos;&apos;b&apos;&quot;,wb.Worksheets[0].PivotTables[0].DataFields[1].GetFormula());
           Assert.AreEqual(&quot;=&apos;w&apos;&apos;e&apos;&quot;,wb.Worksheets[0].PivotTables[0].RowFields[0].PivotItems[2].GetFormula());
            wb.Save(Constants.PivotTableDestPath + &quot;CELLSNET56419.xlsb&quot;);
            wb = new Workbook(Constants.PivotTableDestPath + &quot;CELLSNET56419.xlsb&quot;);
            Assert.AreEqual(&quot;=&apos;b&apos;&apos;b&apos;&quot;, wb.Worksheets[0].PivotTables[0].DataFields[1].GetFormula());
            Assert.AreEqual(&quot;=&apos;w&apos;&apos;e&apos;&quot;, wb.Worksheets[0].PivotTables[0].RowFields[0].PivotItems[2].GetFormula());
            wb.Save(Constants.PivotTableDestPath + &quot;CELLSNET56419.xlsx&quot;);
        }
```

### See Also

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


