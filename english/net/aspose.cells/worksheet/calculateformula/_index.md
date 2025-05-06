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
// Called: Assert.AreEqual(1234.56, sheet.CalculateFormula(fml), fml);
[Test]
        public void Method_String_()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Worksheet sheet = wb.Worksheets[0];
            string fml = &quot;=NUMBERVALUE(\&quot;1.234,56\&quot;,\&quot;,\&quot;)&quot;;
            Assert.AreEqual(1234.56, sheet.CalculateFormula(fml), fml);
            fml = &quot;=NUMBERVALUE(\&quot;1.234,56\&quot;,\&quot;.\&quot;)&quot;;
            Assert.AreEqual(&quot;#VALUE!&quot;, sheet.CalculateFormula(fml), fml);
            fml = &quot;=NUMBERVALUE(\&quot;1.234,56\&quot;)&quot;;
            Assert.AreEqual(&quot;#VALUE!&quot;, sheet.CalculateFormula(fml), fml);
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
// Called: Assert.AreEqual(&amp;quot;#DIV/0!&amp;quot;, sheet.CalculateFormula(fml, copts), fml);
[Test]
        public void Method_CalculationOptions_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells[0, 1].PutValue(&quot;#DIV/0!&quot;);
            string fml = &quot;=LINEST(B1,123)&quot;;
            CalculationOptions copts = new CalculationOptions();
            Assert.AreEqual(&quot;#VALUE!&quot;, sheet.CalculateFormula(fml, copts), fml);
            fml = &quot;=LINEST(#DIV/0!,123)&quot;;
            Assert.AreEqual(&quot;#DIV/0!&quot;, sheet.CalculateFormula(fml, copts), fml);
            fml = &quot;=LINEST(1/0,123)&quot;;
            Assert.AreEqual(&quot;#DIV/0!&quot;, sheet.CalculateFormula(fml, copts), fml);
            fml = &quot;=LINEST(ABS(B1),123)&quot;;
            Assert.AreEqual(&quot;#DIV/0!&quot;, sheet.CalculateFormula(fml, copts), fml);
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
// Called: FormulaCaseUtil.AssertInt(48, sheet.CalculateFormula(&amp;quot;=MYFUNC(B:B+C:C,B:B-C:C,B:B*C:C)&amp;quot;,
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
            FormulaCaseUtil.AssertInt(3, sheet.CalculateFormula(&quot;=MYFUNC(B:B+C:C)&quot;, copts), &quot;ValueMode&quot;);
            ce._arrayMode = true;
            FormulaCaseUtil.AssertInt(15, sheet.CalculateFormula(&quot;=MYFUNC(B:B+C:C)&quot;, copts), &quot;ArrayMode&quot;);

            FormulaParseOptions popts = new FormulaParseOptions();
            popts.CustomFunctionDefinition = new MyCustomFunctionDefinition();
            ce._arrayMode = false;
            ce._autoMode = true;
            FormulaCaseUtil.AssertInt(48, sheet.CalculateFormula(&quot;=MYFUNC(B:B+C:C,B:B-C:C,B:B*C:C)&quot;,
                popts, copts, 0, 0, null), &quot;Parsed ArrayMode&quot;);

            Cell cell = cells[0, 0];
            cell.Formula = &quot;=MYFUNC(B:B+C:C,B:B-C:C,B:B*C:C)&quot;;
            wb.UpdateCustomFunctionDefinition(new MyCustomFunctionDefinition());
            wb.CalculateFormula(copts);
            FormulaCaseUtil.AssertInt(48, cell.Value, &quot;Updated ArrayMode&quot;);
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
// Called: wb.Worksheets[2].CalculateFormula(copts, false);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook();
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            cell.Formula = &quot;=1+2&quot;;
            InterruptCalculationMonitor m = new InterruptCalculationMonitor();
            CalculationOptions copts = new CalculationOptions();
            copts.CalculationMonitor = m;
            wb.CalculateFormula(copts);
            Assert.IsTrue(m.Changed);
            Cells cells = wb.Worksheets.Add(&quot;Sheet2&quot;).Cells;
            m.InterruptedSheet = 1;
            cells[0, 0].Formula = &quot;=B1&quot;;
            cells[2, 1].Formula = &quot;=B4&quot;;
            cells[3, 1].Formula = &quot;=1+2&quot;;
            wb.CalculateFormula(copts);
            Assert.AreEqual(0, cells[0, 0].IntValue, &quot;Sheet2!A1&quot;);
            Assert.IsNull(cells[2, 1].Value, &quot;B3.Value&quot;);
            Assert.IsNull(cells[3, 1].Value, &quot;B4.Value&quot;);
            cells = wb.Worksheets.Add(&quot;Sheet3&quot;).Cells;
            m.InterruptedSheet = 2;
            m.InterruptedMsg = &quot;Interrupted by user&quot;;
            cells[0, 0].Formula = &quot;=B1&quot;;
            cells[2, 1].Formula = &quot;=B4&quot;;
            cells[3, 1].Formula = &quot;=1+2&quot;;
            bool fail = false;
            try
            {
                wb.CalculateFormula(copts);
                fail = true;
            }
            catch (CellsException e)
            {
                if (e.Code != ExceptionType.Interrupted)
                {
                    throw e;
                }
                Console.WriteLine(&quot;As expected for Workbook.CalculateFormula(): &quot; + e.Message);
            }
            if (fail)
            {
                Assert.Fail(&quot;CellsException with ExceptionType.Interrupted was expected for Workbook.CalculateFormula()!&quot;);
            }
            Assert.AreEqual(0, cells[0, 0].IntValue, &quot;Sheet3!A1&quot;);
            Assert.IsNull(cells[2, 1].Value, &quot;Sheet3!B3.Value&quot;);
            Assert.IsNull(cells[3, 1].Value, &quot;Sheet3!B4.Value&quot;);
            fail = false;
            try
            {
                wb.Worksheets[2].CalculateFormula(copts, false);
            }
            catch (CellsException e)
            {
                if (e.Code != ExceptionType.Interrupted)
                {
                    throw e;
                }
                Console.WriteLine(&quot;As expected for Worksheet.CalculateFormula(): &quot; + e.Message);
            }
            if (fail)
            {
                Assert.Fail(&quot;CellsException with ExceptionType.Interrupted was expected for Worksheet.CalculateFormula()!&quot;);
            }
        }
```

### See Also

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


