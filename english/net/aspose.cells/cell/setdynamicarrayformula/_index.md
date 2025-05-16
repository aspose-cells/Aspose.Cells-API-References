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
// Called: cell1.SetDynamicArrayFormula("=SEQUENCE(B2)", new FormulaParseOptions(), true);
public void Cell_Method_SetDynamicArrayFormula()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    Cell cell1 = cells[0, 0];
    cell1.SetDynamicArrayFormula("=SEQUENCE(B2)", new FormulaParseOptions(), true);
    Cell cell2 = cells[1, 1];
    cell2.PutValue(2);
    Cell cell3 = cells[2, 1];
    cell3.Formula = "=A1&A2&A3&A4&A5&A6&A7";
    wb.CalculateFormula();
    Assert.AreEqual("1", cell3.Value);
    wb.RefreshDynamicArrayFormulas(false);
    wb.CalculateFormula();
    Assert.AreEqual("12", cell3.Value);
    cell2.PutValue(5);
    wb.RefreshDynamicArrayFormulas(false);
    wb.CalculateFormula();
    Assert.AreEqual("12345", cell3.Value);
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

### Examples

```csharp
namespace AsposeCellsExamples.CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Get cell C1 where the dynamic array formula will be set
            Cell cell = worksheet.Cells["C1"];

            // Define the dynamic array formula
            string formula = "=A1:B2 * 2";
            
            // Create formula parse options
            FormulaParseOptions options = new FormulaParseOptions
            {
                Parse = true // Enable formula parsing
            };

            // Prepare values to populate the formula result cells
            object[][] values = new object[2][];
            values[0] = new object[] { 2, 4 };
            values[1] = new object[] { 6, 8 };

            try
            {
                // Set dynamic array formula with pre-calculated values
                CellArea result = cell.SetDynamicArrayFormula(
                    formula,
                    options,
                    values,
                    calculateRange: false,  // Use values array dimensions for spill range
                    calculateValue: false  // Use provided values instead of calculating
                );

                Console.WriteLine($"Dynamic array formula set. Affected range: Rows {result.StartRow}-{result.EndRow}, Columns {result.StartColumn}-{result.EndColumn}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetDynamicArrayFormula: {ex.Message}");
            }

            // Save the workbook with the changes
            workbook.Save("SetDynamicArrayFormulaDemo.xlsx");
        }
    }
}
```

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

### Examples

```csharp
namespace AsposeCellsExamples.CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo1
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo1
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate sample data in cells A2:B5
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(60);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B3"].PutValue(55);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["B5"].PutValue(70);

            // Get target cell A1
            Cell cellA1 = worksheet.Cells["A1"];

            try
            {
                // Prepare parameters for SetDynamicArrayFormula
                string formula = "=FILTER(A2:A5, B2:B5>50)";
                FormulaParseOptions options = new FormulaParseOptions { Parse = true };
                object[][] values = new object[2][] { new object[] { 10 }, new object[] { 40 } };
                bool calculateRange = true;
                bool calculateValue = true;
                CalculationOptions calcOptions = new CalculationOptions { Recursive = true };

                // Call SetDynamicArrayFormula with specific parameters
                CellArea spillRange = cellA1.SetDynamicArrayFormula(
                    formula,
                    options,
                    values,
                    calculateRange,
                    calculateValue,
                    calcOptions
                );

                Console.WriteLine($"Dynamic array formula set successfully. Spill range: {spillRange}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetDynamicArrayFormula method: {ex.Message}");
            }

            // Save the result
            workbook.Save("SetDynamicArrayFormulaDemo.xlsx");
        }
    }
}
```

### See Also

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


