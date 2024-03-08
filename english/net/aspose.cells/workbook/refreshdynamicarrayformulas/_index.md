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

### See Also

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


