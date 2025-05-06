---
title: Workbook.RefreshDynamicArrayFormulas
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Refreshes dynamic array formulasspill into new range of neighboring cells according to current data Other formulas in the workbook will not be calculated recursively even if they were used by dynamic array formulas
type: docs
url: /net/aspose.cells/workbook/refreshdynamicarrayformulas/
---
## RefreshDynamicArrayFormulas(bool) {#refreshdynamicarrayformulas}

Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) Other formulas in the workbook will not be calculated recursively even if they were used by dynamic array formulas.

```csharp
public void RefreshDynamicArrayFormulas(bool calculate)
```

| Parameter | Type | Description |
| --- | --- | --- |
| calculate | Boolean | Whether calculates and updates cell values for those dynamic array formulas |

### Examples

```csharp
// Called: wb.RefreshDynamicArrayFormulas(false);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Cell cell1 = cells[0, 0];
            cell1.SetDynamicArrayFormula(&quot;=SEQUENCE(B2)&quot;, new FormulaParseOptions(), true);
            Cell cell2 = cells[1, 1];
            cell2.PutValue(2);
            Cell cell3 = cells[2, 1];
            cell3.Formula = &quot;=A1&amp;A2&amp;A3&amp;A4&amp;A5&amp;A6&amp;A7&quot;;
            wb.CalculateFormula();
            Assert.AreEqual(&quot;1&quot;, cell3.Value);
            wb.RefreshDynamicArrayFormulas(false);
            wb.CalculateFormula();
            Assert.AreEqual(&quot;12&quot;, cell3.Value);
            cell2.PutValue(5);
            wb.RefreshDynamicArrayFormulas(false);
            wb.CalculateFormula();
            Assert.AreEqual(&quot;12345&quot;, cell3.Value);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshDynamicArrayFormulas(bool, CalculationOptions) {#refreshdynamicarrayformulas_1}

Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data)

```csharp
public void RefreshDynamicArrayFormulas(bool calculate, CalculationOptions copts)
```

| Parameter | Type | Description |
| --- | --- | --- |
| calculate | Boolean | Whether calculates and updates cell values for those dynamic array formulas |
| copts | CalculationOptions | The options for calculating formulas |

### Remarks

For performance consideration, we do not refresh all dynamic array formulas automatically when the formula itself or the data it references to changed. So user need to call this method manually after those operations which may influence dynamic array formulas, such as importing/setting cell values, inserting/deleting rows/columns/ranges, ...etc. For most formulas with functions, calculating the spill range also needs to calculating the formula, so in general true value for "calculate" flag is preferred. If the formula is simple, such as a range reference or array(for example "=C1:E5", "={1,2;3,4}", ...), simple function on a range or array(for example "=ABS(C1:E5)", "=1+{1,2;3,4}", ...), and all formulas will be calculated later(such as by [`CalculateFormula`](../calculateformula/)), then using false vlaue for "calculate" flag may avoid the duplicated calculation for the benefit of performance.

### Examples

```csharp
// Called: wb.RefreshDynamicArrayFormulas(true, copts);
[Test]
        public void Method_CalculationOptions_() //CELLSNET-51911
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Cell fc = cells[0, 0];
            Cell dc = cells[&quot;F1&quot;];
            dc.PutValue(&quot;2022-8-31&quot;);
            CalculationOptions copts = new CalculationOptions();
            CalcStockHistory engine = new CalcStockHistory();
            copts.CustomEngine = engine;
            string fml = &quot;=STOCKHISTORY(\&quot;SPY\&quot;,\&quot;2022-8-13\&quot;,F1)&quot;;
            engine.mMsgHeader = &quot;Stage1: &quot;;
            fc.SetDynamicArrayFormula(fml,
                new FormulaParseOptions(), null, true, true, copts);
            CheckStockData(cells, fml, 19, 2, engine.mMsgHeader);
            dc.PutValue(&quot;2022-8-21&quot;);
            engine.mMsgHeader = &quot;Stage2: &quot;;
            wb.RefreshDynamicArrayFormulas(true, copts);
            CheckStockData(cells, fml, 9, 2, engine.mMsgHeader);
            fml = &quot;=STOCKHISTORY(\&quot;SPY\&quot;,\&quot;2022-8-13\&quot;,F1,1,0,2)&quot;;
            engine.mMsgHeader = &quot;Stage3: &quot;;
            fc.SetDynamicArrayFormula(fml,
                new FormulaParseOptions(), null, true, true, copts);
            CheckStockData(cells, fml, 13, 1, engine.mMsgHeader);
            dc.PutValue(&quot;2022-8-31&quot;);
            engine.mMsgHeader = &quot;Stage4: &quot;;
            wb.RefreshDynamicArrayFormulas(true, copts);
            CheckStockData(cells, fml, 23, 1, engine.mMsgHeader);
        }
```

### See Also

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


