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
// Called: object[][] res = sheet.CalculateArrayFormula(fml, copts);
[Test]
        public void Method_CalculationOptions_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            cells[0, 1].PutValue(1);
            cells[1, 1].PutValue(2);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            CalculationOptions copts = new CalculationOptions();
            string fml;
            for (int i = 1; i &lt; 3; i++)
            {
                fml = &quot;=MATCH(&quot; + i + &quot;,COUNTIF(B1:B4,B1:B2))&quot;;
                object[][] res = sheet.CalculateArrayFormula(fml, copts);
                Assert.AreEqual(1, res.Length, &quot;Worksheet.CalculateArrayFormula().Length for &quot; + fml);
                Assert.AreEqual(1, res[0].Length, &quot;Worksheet.CalculateArrayFormula()[0].Length &quot; + fml);
                FormulaCaseUtil.AssertInt(i, res[0][0], &quot;Worksheet.CalculateArrayFormula()&quot;);
                Assert.AreEqual(&quot;#N/A&quot;, sheet.CalculateFormula(fml, copts), &quot;As normal formula for &quot; + fml);
            }

            fml = &quot;=SUM(ABS($B$2:$B$4))&quot;;
            Assert.AreEqual(&quot;#VALUE!&quot;, sheet.CalculateFormula(fml, copts), &quot;As normal formula for &quot; + fml);
            wb.Worksheets.Names.Add(&quot;testname&quot;);
            wb.Worksheets.Names[&quot;testname&quot;].RefersTo = &quot;ABS($B$1:$B$4)&quot;;
            fml = &quot;=SUM(testname)&quot;;
            FormulaCaseUtil.AssertInt(8, sheet.CalculateFormula(fml, copts), &quot;As normal formula for &quot; + fml);

            fml = &quot;=SUM({TRUE})&quot;;
            FormulaCaseUtil.AssertInt(0, sheet.CalculateFormula(fml, copts), &quot;As normal formula for &quot; + fml);
            FormulaCaseUtil.AssertInt(0, ((object[][])sheet.CalculateArrayFormula(fml, copts))[0][0],
                &quot;As array formula for &quot; + fml);
            fml = &quot;=SUM({TRUE,TRUE})&quot;;
            FormulaCaseUtil.AssertInt(0, sheet.CalculateFormula(fml, copts), &quot;As normal formula for &quot; + fml);
            FormulaCaseUtil.AssertInt(0, ((object[][])sheet.CalculateArrayFormula(fml, copts))[0][0],
                &quot;As array formula for &quot; + fml);
            fml = &quot;=SUM(+{TRUE,TRUE})&quot;;
            FormulaCaseUtil.AssertInt(0, sheet.CalculateFormula(fml, copts), &quot;As normal formula for &quot; + fml);
            FormulaCaseUtil.AssertInt(0, ((object[][])sheet.CalculateArrayFormula(fml, copts))[0][0],
                &quot;As array formula for &quot; + fml);
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
// Called: Assert.AreEqual(true, sheet.CalculateArrayFormula(fml, copts, -1, -1)[0][0], fml);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            string fml = &quot;=ISBLANK(+B1)&quot;;
            Assert.AreEqual(true, sheet.CalculateFormula(fml), fml);
            fml = &quot;=ISBLANK(IF(TRUE,B2:B5))&quot;;
            CalculationOptions copts = new CalculationOptions();
            Assert.AreEqual(true, sheet.CalculateArrayFormula(fml, copts, 1, 1)[0][0], fml);
            fml = &quot;=ISBLANK(IF(TRUE,+B2:B5))&quot;;
            Assert.AreEqual(true, sheet.CalculateArrayFormula(fml, copts, -1, -1)[0][0], fml);
            //CELLSNET-54150
            fml = &quot;=ISBLANK(IF({1;2;3;4},B2:B5))&quot;;
            Assert.AreEqual(false, sheet.CalculateArrayFormula(fml, copts, 1, 1)[0][0], fml);
            fml = &quot;=ISBLANK(IF({1;2;3;4},INDIRECT(\&quot;B2:B5\&quot;)))&quot;;
            Assert.AreEqual(false, sheet.CalculateArrayFormula(fml, copts, 1, 1)[0][0], fml);
            fml = &quot;=LEN(IF({1;2;3;4},B2:B5))&quot;;
            FormulaCaseUtil.AssertInt(1, sheet.CalculateArrayFormula(fml, copts, 1, 1)[0][0], fml);
            fml = &quot;=MATCH(0,IF(B2:B5=5,C2:C5,D2:D5),0)&quot;;
            FormulaCaseUtil.AssertInt(1, sheet.CalculateArrayFormula(fml, copts, 1, 1)[0][0], fml);
            //CELLSJAVA-45592
            fml = &quot;=MATCH(1,IF(B2:B5=5,C2:C5,D2:D5),0)&quot;;
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


