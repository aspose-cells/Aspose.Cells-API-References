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

### Examples

```csharp
// Called: Assert.AreEqual(0.017361111, (double)sheet.CalculateFormula(fml), 1.0E-7, fml);
public void Worksheet_Method_CalculateFormula()
{
    Workbook wb = new Workbook();
    wb.Settings.Region = CountryCode.USA;
    Worksheet sheet = wb.Worksheets[0];
    string fml = "=NUMBERVALUE(\"\")";
    FormulaCaseUtil.AssertInt(0, sheet.CalculateFormula(fml), fml);
    fml = "=NUMBERVALUE(\" \")";
    FormulaCaseUtil.AssertInt(0, sheet.CalculateFormula(fml), fml);
    fml = "=NUMBERVALUE(\"1 2  3\")";
    FormulaCaseUtil.AssertInt(123, sheet.CalculateFormula(fml), fml);
    fml = "=NUMBERVALUE(\"$1.234\")";
    Assert.AreEqual(1.234, (double)sheet.CalculateFormula(fml), 1.0E-7, fml);
    fml = "=NUMBERVALUE(\"$1,234.567\")";
    Assert.AreEqual(1234.567, (double)sheet.CalculateFormula(fml), 1.0E-7, fml);
    fml = "=NUMBERVALUE(\"0:25\")";
    Assert.AreEqual(0.017361111, (double)sheet.CalculateFormula(fml), 1.0E-7, fml);
    fml = "=NUMBERVALUE(\"07/26/2023\")";
    FormulaCaseUtil.AssertInt(45133, sheet.CalculateFormula(fml), fml);
    fml = "=NUMBERVALUE(\"26/07/2023\")";
    Assert.AreEqual("#VALUE!", (string)sheet.CalculateFormula(fml), fml);
    fml = "=NUMBERVALUE(\"15:23:25\")";
    Assert.AreEqual(0.641261574, (double)sheet.CalculateFormula(fml), 1.0E-7, fml);
    fml = "=NUMBERVALUE(\"07/26/2023 15:23:25\")";
    Assert.AreEqual("#VALUE!", (string)sheet.CalculateFormula(fml), fml);
    //Assert.AreEqual(45133.641261574, (double)v, 1.0E-7, fml);
}
```

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

### Examples

```csharp
// Called: object o = wb.Worksheets[0].CalculateFormula("=CUSTOMFUNC()",
public void Worksheet_Method_CalculateFormula()
{
    Workbook wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];
    Cells cells = sheet.Cells;
    cells[1, 0].PutValue("#VALUE!");
    cells[2, 0].PutValue(1);
    cells[3, 0].PutValue(2);
    cells[1, 1].PutValue(11);
    cells[2, 1].PutValue(12);
    cells[3, 1].PutValue(13);
    CE53317 ce = new CE53317();
    object o = wb.Worksheets[0].CalculateFormula("=CUSTOMFUNC()",
        new CalculationOptions() { CustomEngine = ce });
    Assert.AreEqual(0, ce.CellRow, "BaseRow");
    Assert.AreEqual(0, ce.CellColumn, "BaseColumn");
    Assert.IsNull(ce.BaseCell, "BaseCell");
    object[][] arr = (object[][])o;
    Assert.AreEqual(3, arr.Length);
    for (int i = 0; i < 3; i++)
    {
        object[] item = arr[i];
        Assert.AreEqual(1, item.Length);
        Assert.AreEqual(i == 0 ? 11 : i,
            item[0] is double ? (int)(double)item[0] : (int)item[0], "Result-" + i);
    }
}
```

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

### Examples

```csharp
// Called: FormulaCaseUtil.AssertInt(48, sheet.CalculateFormula("=MYFUNC(B:B+C:C,B:B-C:C,B:B*C:C)",
public void Worksheet_Method_CalculateFormula()
{
    Workbook wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];
    Cells cells = sheet.Cells;
    cells[0, 1].PutValue(1);
    cells[0, 2].PutValue(2);
    cells[1, 1].PutValue(4);
    cells[1, 2].PutValue(8);
    ArrayModeParamEngine ce = new ArrayModeParamEngine();
    CalculationOptions copts = new CalculationOptions();
    copts.CustomEngine = ce;
    FormulaCaseUtil.AssertInt(3, sheet.CalculateFormula("=MYFUNC(B:B+C:C)", copts), "ValueMode");
    ce._arrayMode = true;
    FormulaCaseUtil.AssertInt(15, sheet.CalculateFormula("=MYFUNC(B:B+C:C)", copts), "ArrayMode");

    FormulaParseOptions popts = new FormulaParseOptions();
    popts.CustomFunctionDefinition = new MyCustomFunctionDefinition();
    ce._arrayMode = false;
    ce._autoMode = true;
    FormulaCaseUtil.AssertInt(48, sheet.CalculateFormula("=MYFUNC(B:B+C:C,B:B-C:C,B:B*C:C)",
        popts, copts, 0, 0, null), "Parsed ArrayMode");

    Cell cell = cells[0, 0];
    cell.Formula = "=MYFUNC(B:B+C:C,B:B-C:C,B:B*C:C)";
    wb.UpdateCustomFunctionDefinition(new MyCustomFunctionDefinition());
    wb.CalculateFormula(copts);
    FormulaCaseUtil.AssertInt(48, cell.Value, "Updated ArrayMode");
}
```

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

### Examples

```csharp
// Called: sheet.CalculateFormula(opts, true);
public void Worksheet_Method_CalculateFormula()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    int activeIndex = wb.Worksheets.ActiveSheetIndex;

    CalculationOptions opts = new CalculationOptions();
    opts.Recursive = true;
    opts.IgnoreError = false;
    wb.CalculateFormula(opts);
    Worksheet sheet = wb.Worksheets[activeIndex];
    sheet.CalculateFormula(opts, true);

    sheet.Shapes.UpdateSelectedValue();
    wb.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


