---
title: Cell.Calculate
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Calculates the formula of the cell
type: docs
url: /net/aspose.cells/cell/calculate/
---
## Cell.Calculate method

Calculates the formula of the cell.

```csharp
public void Calculate(CalculationOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | CalculationOptions | Options for calculation |

### Examples

```csharp
// Called: cell.Calculate(new CalculationOptions());
[Test]
        public void Method_CalculationOptions_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            wb.Worksheets.Names.Add(&quot;MyTestName&quot;);
            Name n = wb.Worksheets.Names[0];
            cells[0, 0].PutValue(1);
            cells[0, 1].PutValue(2);
            cells[0, 2].PutValue(4);
            Cell cell = cells[2, 0];
            cell.Formula = &quot;=SUM(INDIRECT(\&quot;MyTestName#\&quot;))&quot;;

            n.RefersTo = &quot;=Sheet1!$A$1:$B$1&quot;;
            cell.Calculate(new CalculationOptions());
            FormulaCaseUtil.AssertInt(3, cell.Value, &quot;DefinedName(Range)# for non-dynamic&quot;);

            n.RefersTo = &quot;=Sheet1!$A$1&quot;;
            cell.Calculate(new CalculationOptions());
            Assert.AreEqual(&quot;#REF!&quot;, cell.Value, &quot;DefinedName(Cell)# for non-dynamic&quot;);

            cells[1, 0].SetDynamicArrayFormula(&quot;=A1:C1&quot;, new FormulaParseOptions(), true);

            n.RefersTo = &quot;=Sheet1!$A$2&quot;;
            cell.Calculate(new CalculationOptions());
            FormulaCaseUtil.AssertInt(7, cell.Value, &quot;DefinedName(Cell)# for dynamic&quot;);

            n.RefersTo = &quot;=Sheet1!$A$2:$B$2&quot;;
            cell.Calculate(new CalculationOptions());
            FormulaCaseUtil.AssertInt(3, cell.Value, &quot;DefinedName(Range)# for dynamic&quot;);
        }
```

### See Also

* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


