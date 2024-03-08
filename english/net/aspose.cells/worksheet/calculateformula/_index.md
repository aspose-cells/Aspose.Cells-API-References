---
title: Worksheet.CalculateFormula
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Calculates a formula
type: docs
url: /net/aspose.cells/worksheet/calculateformula/
---
## CalculateFormula(string) {#calculateformula}

Calculates a formula.

```csharp
public object CalculateFormula(string formula)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |

### Return Value

Calculated formula result.

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(string, CalculationOptions) {#calculateformula_1}

Calculates a formula expression directly.

```csharp
public object CalculateFormula(string formula, CalculationOptions opts)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| opts | CalculationOptions | Options for calculating formula |

### Return Value

Calculated result of given formula. The returned object may be of possible types of [`Value`](../../cell/value/), or ReferredArea.

### Remarks

The formula will be calculated just like it has been set to cell A1. And the formula will be taken as normal formula. If you need the formula be calculated as an array formula and to get an array for the calculated result, please use [`CalculateArrayFormula`](../calculatearrayformula/) instead.

### See Also

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(string, FormulaParseOptions, CalculationOptions, int, int, CalculationData) {#calculateformula_2}

Calculates a formula expression directly.

```csharp
public object CalculateFormula(string formula, FormulaParseOptions pOpts, CalculationOptions cOpts, 
    int baseCellRow, int baseCellColumn, CalculationData calculationData)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| pOpts | FormulaParseOptions | Options for parsing formula. |
| cOpts | CalculationOptions | Options for calculating formula. |
| baseCellRow | Int32 | The row index of the base cell. |
| baseCellColumn | Int32 | The column index of the base cell. |
| calculationData | CalculationData | The calculation data. It is used for the situation that user needs to calculate some static formulas when implementing custom calculation engine. For such kind of situation, user needs to specify it with the calculation data provided for [`Calculate`](../../abstractcalculationengine/calculate/). |

### Return Value

Calculated result of given formula. The returned object may be of possible types of [`Value`](../../cell/value/), or ReferredArea.

### Remarks

The formula will be calculated just like it has been set to the specified base cell. And the formula will be taken as normal formula. If you need the formula be calculated as an array formula and to get an array for the calculated result, please use [`CalculateArrayFormula`](../calculatearrayformula/) instead.

### See Also

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(CalculationOptions, bool) {#calculateformula_3}

Calculates all formulas in this worksheet.

```csharp
public void CalculateFormula(CalculationOptions options, bool recursive)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | CalculationOptions | Options for calculation |
| recursive | Boolean | True means if the worksheet' cells depend on the cells of other worksheets, the dependent cells in other worksheets will be calculated too. False means all the formulas in the worksheet have been calculated and the values are right. |

### See Also

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


