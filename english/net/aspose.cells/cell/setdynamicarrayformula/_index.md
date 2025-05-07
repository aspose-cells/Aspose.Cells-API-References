---
title: Cell.SetDynamicArrayFormula
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Sets dynamic array formula and make the formula spill into neighboring cells if possible
type: docs
url: /net/aspose.cells/cell/setdynamicarrayformula/
---
## SetDynamicArrayFormula(string, FormulaParseOptions, bool) {#setdynamicarrayformula}

Sets dynamic array formula and make the formula spill into neighboring cells if possible.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    bool calculateValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | the formula expression |
| options | FormulaParseOptions | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| calculateValue | Boolean | whether calculate this dynamic array formula for those cells in the spilled range. |

### Return Value

the range that the formula should spill into.

### Remarks

the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.

### Examples

```csharp
// Called: cells[0, 1].SetDynamicArrayFormula("=MAP({1;2},LAMBDA(x,x+1))", new FormulaParseOptions(), true);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Cell cell = cells[0, 0];
            cell.SetDynamicArrayFormula("=MAP({3;4},LAMBDA(x,B1+x))", new FormulaParseOptions(), false);
            cells[0, 1].SetDynamicArrayFormula("=MAP({1;2},LAMBDA(x,x+1))", new FormulaParseOptions(), true);
            wb.CalculateFormula();
            FormulaCaseUtil.AssertInt(5, cell.Value, "LAMBDA used in cells which need to be calculated recursively");
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool) {#setdynamicarrayformula_1}

Sets dynamic array formula and make the formula spill into neighboring cells if possible.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    object[][] values, bool calculateRange, bool calculateValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | the formula expression |
| options | FormulaParseOptions | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| values | Object[][] | values(calculated results) for those cells with given dynamic array formula |
| calculateRange | Boolean | Whether calculate the spilled range for this dynamic array formula. If the "values" parameter is not null and this flag is false, then the spilled range's height will be values.Length and width will be values[0].Length. |
| calculateValue | Boolean | whether calculate this dynamic array formula for those cells in the spilled range when "values" is null or corresponding item in "values" for one cell is null. |

### Return Value

the range that the formula should spill into.

### Remarks

the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.

### See Also

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool, CalculationOptions) {#setdynamicarrayformula_2}

Sets dynamic array formula and make the formula spill into neighboring cells if possible.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    object[][] values, bool calculateRange, bool calculateValue, CalculationOptions copts)
```

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | the formula expression |
| options | FormulaParseOptions | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| values | Object[][] | values(calculated results) for those cells with given dynamic array formula |
| calculateRange | Boolean | Whether calculate the spilled range for this dynamic array formula. If the "values" parameter is not null and this flag is false, then the spilled range's height will be values.Length and width will be values[0].Length. |
| calculateValue | Boolean | whether calculate this dynamic array formula for those cells in the spilled range when "values" is null or corresponding item in "values" for one cell is null. |
| copts | CalculationOptions | The options for calculating formula. Commonly, for performance consideration, the [`Recursive`](../../calculationoptions/recursive/) property should be false. |

### Return Value

the range that the formula should spill into.

### Remarks

the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.

### See Also

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


