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
// Called: FormulaCaseUtil.AssertInt(28, sheet.CalculateArrayFormula(fml, new CalculationOptions())[0][0], fml);
public void Worksheet_Method_CalculateArrayFormula()
{
    Workbook wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];
    Cells cells = sheet.Cells;
    cells[0, 0].PutValue(1);
    cells[0, 1].PutValue(2);
    cells[0, 2].PutValue(3);
    cells[1, 1].PutValue(4);
    cells[1, 2].PutValue(5);
    cells[2, 0].PutValue(6);
    cells[2, 2].PutValue(7);

    string fml = "=UNIQUE(HSTACK(ABS(A1:B3),C1:C3))"; //endless when calculating it
    CellArea expected = CellArea.CreateCellArea(4, 0, 6, 2);
    CellArea ca = cells[4, 0].SetDynamicArrayFormula(fml, new FormulaParseOptions(), true);
    AssertHelper.checkCellArea(expected, ca, fml);
    CheckArrayFormula(fml, cells, ca, "");
    CheckResult(new string[] {
        "1", "2", "3", "0", "4", "5", "6", "0", "7",
    }, cells, ca, "");

    fml = "=SUM(HSTACK(ABS(A1:B3),C1:C3))";
    FormulaCaseUtil.AssertInt(28, sheet.CalculateArrayFormula(fml, new CalculationOptions())[0][0], fml);
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
// Called: Assert.AreEqual(true, sheet.CalculateArrayFormula(fml, copts, 1, 1)[0][0], fml);
public void Worksheet_Method_CalculateArrayFormula()
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


