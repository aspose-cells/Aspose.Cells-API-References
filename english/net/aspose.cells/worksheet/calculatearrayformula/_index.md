---
title: Worksheet.CalculateArrayFormula
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Calculates a formula as array formula
type: docs
url: /net/aspose.cells/worksheet/calculatearrayformula/
---
## CalculateArrayFormula(string, CalculationOptions) {#calculatearrayformula}

Calculates a formula as array formula.

```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| opts | CalculationOptions | Options for calculating formula |

### Examples

```csharp
// Called: object[][] res = sheet.CalculateArrayFormula(fml, new CalculationOptions());
[Test]
        public void Method_CalculationOptions_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            string fml = "=SUMPRODUCT(XLOOKUP({1,2,3},{1,2},{100,200},-1))";
            object[][] res = sheet.CalculateArrayFormula(fml, new CalculationOptions());
            Assert.AreEqual(1, res.Length, "Worksheet.CalculateArrayFormula().Length");
            Assert.AreEqual(1, res[0].Length, "Worksheet.CalculateArrayFormula()[0].Length");
            FormulaCaseUtil.AssertInt(299, res[0][0], "Worksheet.CalculateArrayFormula()");
            FormulaCaseUtil.AssertInt(299, sheet.CalculateFormula(fml), "Worksheet.CalculateFormula()");
        }
```

### See Also

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateArrayFormula(string, CalculationOptions, int, int) {#calculatearrayformula_1}

Calculates a formula as array formula.

```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts, int maxRowCount, 
    int maxColumnCount)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| opts | CalculationOptions | Options for calculating formula |
| maxRowCount | Int32 | the maximum row count of resultant data. If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | Int32 | the maximum column count of resultant data. If it is non-positive or greater than the actual row count, then actual column count will be used. |

### Return Value

Calculated formula result.

### Remarks

The formula will be taken as dynamic array formula to calculate the dimension and result. User specified maximum dimension is used for cases that the calculated result is large data set (for example, the calculated result may correspond to a whole row or column data) but user does not need so large an array according to business requirement or for performance consideration.

### Examples

```csharp
// Called: Assert.AreEqual(false, sheet.CalculateArrayFormula(fml, copts, 1, 1)[0][0], fml);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            string fml = "=ISBLANK(+B1)";
            Assert.AreEqual(true, sheet.CalculateFormula(fml), fml);
            fml = "=ISBLANK(IF(TRUE,B2:B5))";
            CalculationOptions copts = new CalculationOptions();
            Assert.AreEqual(true, sheet.CalculateArrayFormula(fml, copts, 1, 1)[0][0], fml);
            fml = "=ISBLANK(IF(TRUE,+B2:B5))";
            Assert.AreEqual(true, sheet.CalculateArrayFormula(fml, copts, -1, -1)[0][0], fml);
            //CELLSNET-54150
            fml = "=ISBLANK(IF({1;2;3;4},B2:B5))";
            Assert.AreEqual(false, sheet.CalculateArrayFormula(fml, copts, 1, 1)[0][0], fml);
            fml = "=ISBLANK(IF({1;2;3;4},INDIRECT(\"B2:B5\")))";
            Assert.AreEqual(false, sheet.CalculateArrayFormula(fml, copts, 1, 1)[0][0], fml);
            fml = "=LEN(IF({1;2;3;4},B2:B5))";
            FormulaCaseUtil.AssertInt(1, sheet.CalculateArrayFormula(fml, copts, 1, 1)[0][0], fml);
            fml = "=MATCH(0,IF(B2:B5=5,C2:C5,D2:D5),0)";
            FormulaCaseUtil.AssertInt(1, sheet.CalculateArrayFormula(fml, copts, 1, 1)[0][0], fml);
            //CELLSJAVA-45592
            fml = "=MATCH(1,IF(B2:B5=5,C2:C5,D2:D5),0)";
            Cells cells = sheet.Cells;
            cells[3, 1].PutValue(5);
            cells[3, 2].PutValue(1);
            FormulaCaseUtil.AssertInt(3, sheet.CalculateArrayFormula(fml, copts, 1, 1)[0][0], fml);
        }
```

### See Also

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateArrayFormula(string, FormulaParseOptions, CalculationOptions, int, int, int, int, CalculationData) {#calculatearrayformula_2}

Calculates a formula as array formula.

```csharp
public object[][] CalculateArrayFormula(string formula, FormulaParseOptions pOpts, 
    CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, 
    int maxColumnCount, CalculationData calculationData)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | Formula to be calculated. |
| pOpts | FormulaParseOptions | Options for parsing formula |
| cOpts | CalculationOptions | Options for calculating formula |
| baseCellRow | Int32 | The row index of the base cell. |
| baseCellColumn | Int32 | The column index of the base cell. |
| maxRowCount | Int32 | The maximum row count of resultant data. If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | Int32 | The maximum column count of resultant data. If it is non-positive or greater than the actual row count, then actual column count will be used. |
| calculationData | CalculationData | The calculation data. It is used for the situation that user needs to calculate some static formulas when implementing custom calculation engine. For such kind of situation, user needs to specify it with the calculation data provided for [`Calculate`](../../abstractcalculationengine/calculate/). |

### Return Value

Calculated formula result.

### Remarks

The formula will be taken as dynamic array formula to calculate the dimension and result. User specified maximum dimension is used for cases that the calculated result is large data set (for example, the calculated result may correspond to a whole row or column data) but user does not need so large an array according to business requirement or for performance consideration.

### See Also

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


