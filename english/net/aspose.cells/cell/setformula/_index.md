---
title: Cell.SetFormula
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Set the formula and the valuecalculated result of the formula
type: docs
url: /net/aspose.cells/cell/setformula/
---
## SetFormula(string, object) {#setformula_3}

Set the formula and the value(calculated result) of the formula.

```csharp
public void SetFormula(string formula, object value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The formula. |
| value | Object | The value(calculated result) of the formula. |

### Examples

```csharp
// Called: cells[0, 1].SetFormula("=SUM(1,2)", 4);
public void Cell_Method_SetFormula()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    cells[0, 0].SetFormula("=MYFUNC()", "OriginalValue");
    cells[0, 1].SetFormula("=SUM(1,2)", 4);
    wb.CalculateFormula(new CalculationOptions() { CustomEngine = new CustomEnginJ45190(null) });
    Assert.AreEqual("OriginalValue", cells[0, 0].StringValue, "IgnoreCalculatingCustomFunction: MYFUNC");
    Assert.AreEqual(4, cells[0, 1].IntValue, "IgnoreCalculatingCustomFunction: SUM");
    object[] buffer = new object[2];
    wb.CalculateFormula(new CalculationOptions() { CustomEngine = new CustomEnginJ45190(buffer) });
    Assert.AreEqual("#NAME?", buffer[0], "CallBuiltInEngine: MYFUNC");
    Assert.AreEqual(3, buffer[1], "CallBuiltInEngine: SUM");
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, FormulaParseOptions) {#setformula}

Set the formula and the value(calculated result) of the formula.

```csharp
public void SetFormula(string formula, FormulaParseOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The formula. |
| options | FormulaParseOptions | Options for parsing the formula. |

### Examples

```csharp
// Called: cell.SetFormula(fml, po);
public void Cell_Method_SetFormula()
{
    Workbook wb = new Workbook(FileFormatType.Xlsx);
    Cell cell = wb.Worksheets[0].Cells[1, 0];
    Cell_Method_SetFormula(cell, "=SUM(A1)(B1:B2)",
        "Non-Reference function cannot be supported to be taken as function name");
    Cell_Method_SetFormula(cell, "=RC()",
        "RC format reference function cannot be supported to be taken as function name");
    Cell_Method_SetFormula(cell, "=R1C()",
        "RC format reference function cannot be supported to be taken as function name");
    FormulaParseOptions po = new FormulaParseOptions();
    po.R1C1Style = true;
    string fml = "=RC()";
    cell.SetFormula(fml, po);
    Assert.AreEqual("=A2()", cell.Formula, "RC formula: " + fml);
    fml = "=R1C()";
    cell.SetFormula(fml, po);
    Assert.AreEqual("=A$1()", cell.Formula, "RC formula: " + fml);
    fml = "=R()";
    cell.SetFormula(fml, po);
    Assert.AreEqual("=2:2()", cell.Formula, "RC formula: " + fml);

    //CELLSNET-56671
    fml = "=SUM1()";
    cell.Formula = fml;
    cell.Calculate(new CalculationOptions());
    Assert.AreEqual("#REF!", cell.Value, "(Xlsx)Calculated value of: " + fml);
    wb.FileFormat = FileFormatType.Excel97To2003;
    cell.Calculate(new CalculationOptions());
    Assert.AreEqual("=#REF!()", cell.Formula, "After converting xlsx to xls: " + fml);
    Assert.AreEqual("#REF!", cell.Value, "(Xlsx)Calculated value of: " + fml);
    cell.Formula = fml;
    cell.Calculate(new CalculationOptions());
    Assert.AreEqual("#NAME?", cell.Value, "(Xls)Calculated value of: " + fml);
}
```

### See Also

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, bool, bool, object) {#setformula_2}

Set the formula and the value of the formula.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetFormula(string formula, bool isR1C1, bool isLocal, object value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The formula. |
| isR1C1 | Boolean | Whether the formula is R1C1 formula. |
| isLocal | Boolean | Whether the formula is locale formatted. |
| value | Object | The value of the formula. |

### Remarks

NOTE: This class is now obsolete. Instead, please use Cell.SetFormula(string,FormulaParseOptions,object). This property will be removed 12 months later since December 2019. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples.CellMethodSetFormulaWithStringBooleanBooleanObjectDemo
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetFormulaWithStringBooleanBooleanObjectDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepare data in cell B2 (row 1, column 1)
            worksheet.Cells[1, 1].PutValue(5);

            // Get cell A1 where we'll set the formula
            Cell cellA1 = worksheet.Cells[0, 0];

            try
            {
                // Call SetFormula with parameters: R1C1-style formula, not localized, null fallback value
                cellA1.SetFormula("=R[1]C[1]*2", true, false, null);

                // Calculate workbook to resolve formula
                workbook.CalculateFormula();

                // Display results
                Console.WriteLine($"Formula set successfully. A1 value: {cellA1.StringValue}");
                Console.WriteLine($"Calculated result: {cellA1.Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula: {ex.Message}");
            }

            // Save the workbook
            workbook.Save("CellSetFormulaDemo.xlsx");
        }
    }
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, FormulaParseOptions, object) {#setformula_1}

Set the formula and the value(calculated result) of the formula.

```csharp
public void SetFormula(string formula, FormulaParseOptions options, object value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The formula. |
| options | FormulaParseOptions | Options for parsing the formula. |
| value | Object | The value(calculated result) of the formula. |

### Examples

```csharp
// Called: sheet.Cells[0, 0].SetFormula("=dsfun(B1)", new FormulaParseOptions() { CheckAddIn = false }, null);
public void Cell_Method_SetFormula()
{
    Workbook wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];
    sheet.Cells[0, 0].Formula = "'externalDS.xlam'!dsfun(B1)";
    Assert.AreEqual("=externalDS.xlam!dsfun(B1)", sheet.Cells[0, 0].Formula);
    sheet.Cells[0, 0].SetFormula("=dsfun(B1)", new FormulaParseOptions() { CheckAddIn = false }, null);
    Assert.AreEqual("=dsfun(B1)", sheet.Cells[0, 0].Formula);

    sheet.Cells[0, 0].Formula = "'externalDS.xlam'!dsfun(B1)";
    Assert.AreEqual("=externalDS.xlam!dsfun(B1)", sheet.Cells[0, 0].Formula);
    wb = new Workbook();
    wb.Worksheets[0].Cells[0, 0].Formula = "'externalDS.xlam'!dsfunnew(C1)";
    wb.Worksheets[0].Copy(sheet);
    Assert.AreEqual("=externalDS.xlam!dsfun(B1)", wb.Worksheets[0].Cells[0, 0].Formula);
}
```

### See Also

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


