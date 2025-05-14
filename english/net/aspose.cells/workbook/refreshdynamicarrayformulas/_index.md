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
// Called: wb.RefreshDynamicArrayFormulas(k == 0);
public void Workbook_Method_RefreshDynamicArrayFormulas()
{
    for (int k = 0; k < 2; k++)
    {
        Workbook wb = new Workbook();
        Cells cells1, cells2;
        if (k == 0)
        {
            cells1 = wb.Worksheets[0].Cells;
            cells2 = wb.Worksheets.Add("Sheet2").Cells;
        }
        else
        {
            cells2 = wb.Worksheets[0].Cells;
            cells1 = wb.Worksheets.Add("Sheet2").Cells;
        }
        Cell cell = cells1[0, 0];
        cell.PutValue("B1:B3");
        cells1[1, 0].SetDynamicArrayFormula("=INDIRECT(A1)", new FormulaParseOptions(), k == 0);
        cells2[0, 1].SetDynamicArrayFormula("=TRANSPOSE(Sheet" + (k + 1) + "!A2#)", new FormulaParseOptions(), k == 0);
        for (int j = 0; j < 2; j++)
        {
            for (int i = 1; i < 5; i++)
            {
                if (i < 4)
                {
                    Cell c = j == 0 ? cells1.CheckCell(i, 0) : cells2.CheckCell(0, i);
                    if (c == null || !c.IsFormula)
                    {
                        Assert.Fail("After setting, " + k + "-" + j + "-" + i + " should be spilled as formula");
                    }
                }
                else
                {
                    Cell c = j == 0 ? cells1.CheckCell(i, 0) : cells2.CheckCell(0, i);
                    if (c != null && c.IsFormula)
                    {
                        Assert.Fail("After setting, " + k + "-" + j + "-" + i + " should not be spilled as formula");
                    }
                }
            }
        }
        cell.PutValue("B1:B5");
        wb.RefreshDynamicArrayFormulas(k == 0);
        for (int j = 0; j < 2; j++)
        {
            for (int i = 1; i < 7; i++)
            {
                if (i < 6)
                {
                    Cell c = j == 0 ? cells1.CheckCell(i, 0) : cells2.CheckCell(0, i);
                    if (c == null || !c.IsFormula)
                    {
                        Assert.Fail("After refresh, " + k + "-" + j + "-" + i + " should be spilled as formula");
                    }
                }
                else
                {
                    Cell c = j == 0 ? cells1.CheckCell(i, 0) : cells2.CheckCell(0, i);
                    if (c != null && c.IsFormula)
                    {
                        Assert.Fail("After refresh, " + k + "-" + j + "-" + i + " should not be spilled as formula");
                    }
                }
            }
        }
    }
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
// Called: excelCalc.RefreshDynamicArrayFormulas(true, opts);
public static void Workbook_Method_RefreshDynamicArrayFormulas(Workbook excelCalc, CalculationOptions opts, CultureInfo ci)
        {
            if (ci != null)
            {
                excelCalc.Settings.CultureInfo = ci;
            }
            //excelCalc.ClearFormulaValues();
            excelCalc.RefreshDynamicArrayFormulas(true, opts);
            excelCalc.CalculateFormula(opts);
        }
```

### See Also

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


