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
// Called: Assert.AreEqual("#VALUE!", sheet.CalculateFormula(fml), fml);
[Test]
        public void Method_String_()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Worksheet sheet = wb.Worksheets[0];
            string fml = "=NUMBERVALUE(\"1.234,56\",\",\")";
            Assert.AreEqual(1234.56, sheet.CalculateFormula(fml), fml);
            fml = "=NUMBERVALUE(\"1.234,56\",\".\")";
            Assert.AreEqual("#VALUE!", sheet.CalculateFormula(fml), fml);
            fml = "=NUMBERVALUE(\"1.234,56\")";
            Assert.AreEqual("#VALUE!", sheet.CalculateFormula(fml), fml);
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
// Called: Assert.AreEqual(6.0, wb.Worksheets[0].CalculateFormula("=USEDECIMAL(3.0)",
[Test]
        public void Method_CalculationOptions_()
        {
            Workbook wb = new Workbook();
            Assert.AreEqual(6.0, wb.Worksheets[0].CalculateFormula("=USEDECIMAL(3.0)",
                new CalculationOptions() { CustomEngine = new CustomEngineSimple() }), "Calculated value");
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
[Test]
        public void Method_CalculationData_()
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
// Called: excelDocument.Worksheets[2].CalculateFormula(new CalculationOptions(), true);
[Test]
        public void Method_Boolean_()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET43667_";
            var excelDocument = new Workbook(filePath + "PivotFormula.xlsx");
            var worksheet = excelDocument.Worksheets[0];
            var value = worksheet.Cells["J5"].DisplayStringValue;
            Console.WriteLine("Before Worksheet.CalculateFormula: {0}", value);

            worksheet.CalculateFormula(new CalculationOptions(), true);
            Assert.AreEqual(value, worksheet.Cells["J5"].DisplayStringValue);
            value = worksheet.Cells["J5"].DisplayStringValue;
            Console.WriteLine("After Worksheet.CalculateFormula: {0}", value);

            excelDocument = new Workbook(filePath + "demo.xlsx");
            value = excelDocument.Worksheets[2].Cells["B2"].StringValue;
            var value2 = excelDocument.Worksheets[2].Cells["B3"].StringValue;
            excelDocument.Worksheets[2].CalculateFormula(new CalculationOptions(), true);
            Assert.AreEqual(value, excelDocument.Worksheets[2].Cells["B2"].DisplayStringValue);
            Assert.AreEqual(value2, excelDocument.Worksheets[2].Cells["B3"].DisplayStringValue);
        }
```

### See Also

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


