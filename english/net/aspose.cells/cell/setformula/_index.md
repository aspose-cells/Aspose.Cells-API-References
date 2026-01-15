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
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringObjectDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Set formula with string and object parameters
            cells["A1"].SetFormula("=SUM(1,2)", 4); // Will display 4 until calculation
            cells["A2"].SetFormula("=AVERAGE(5,10)", 7.5); // Will display 7.5 until calculation

            // Display values before calculation
            Console.WriteLine("Before Calculation:");
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("A2: " + cells["A2"].StringValue);

            // Calculate formulas
            workbook.CalculateFormula();

            // Display values after calculation
            Console.WriteLine("\nAfter Calculation:");
            Console.WriteLine("A1: " + cells["A1"].IntValue); // Should show 3
            Console.WriteLine("A2: " + cells["A2"].DoubleValue); // Should show 7.5
        }
    }
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
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringFormulaParseOptionsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Get a specific cell (B2 in this case)
            Cell cell = worksheet.Cells["B2"];
            
            // Set some initial values for demonstration
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].PutValue(30);
            
            // Example 1: Set a simple formula with default parse options
            cell.SetFormula("=SUM(A1:A2)", new FormulaParseOptions());
            Console.WriteLine("Formula with default options: " + cell.Formula);
            
            // Example 2: Set formula with R1C1 style using FormulaParseOptions
            FormulaParseOptions options = new FormulaParseOptions();
            options.Parse = true;
            options.R1C1Style = true;
            
            cell.SetFormula("=SUM(R[-1]C[-1]:R[0]C[-1])", options);
            Console.WriteLine("Formula with R1C1 style: " + cell.Formula);
            
            // Example 3: Set formula with parse options that preserve the R1C1 format
            options = new FormulaParseOptions();
            options.Parse = true;
            options.R1C1Style = true;
            cell.SetFormula("=R1C1+R2C2", options);
            Console.WriteLine("Formula preserved as R1C1: " + cell.Formula);
            
            // Calculate the workbook to see results
            workbook.CalculateFormula();
            Console.WriteLine("Calculated value: " + cell.Value);
        }
    }
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
namespace AsposeCellsExamples
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

            // Add some sample data
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].PutValue(30);
            worksheet.Cells["B2"].PutValue(40);

            // Get the target cell where we'll set the formula
            Cell cell = worksheet.Cells["C1"];

            try
            {
                // Set a formula with all parameters
                // Parameters: formula string, isR1C1, isLocal, value
                cell.SetFormula("=SUM(A1:B2)", false, false, null);

                // Calculate the formula
                workbook.CalculateFormula();

                // Display the result
                Console.WriteLine($"Formula set successfully. Result: {cell.Value}");

                // Save the workbook
                workbook.Save("SetFormulaDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting formula: {ex.Message}");
            }
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
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringFormulaParseOptionsObjecDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Set initial formula with add-in reference
            sheet.Cells[0, 0].Formula = "'externalDS.xlam'!dsfun(B1)";
            Console.WriteLine("Initial formula: " + sheet.Cells[0, 0].Formula);

            // Use SetFormula to override without checking add-in
            sheet.Cells[0, 0].SetFormula("=dsfun(B1)", new FormulaParseOptions() { CheckAddIn = false }, null);
            Console.WriteLine("After SetFormula: " + sheet.Cells[0, 0].Formula);

            // Reset to add-in formula
            sheet.Cells[0, 0].Formula = "'externalDS.xlam'!dsfun(B1)";
            Console.WriteLine("Reset to add-in formula: " + sheet.Cells[0, 0].Formula);

            // Create new workbook and copy sheet
            Workbook wb2 = new Workbook();
            wb2.Worksheets[0].Cells[0, 0].Formula = "'externalDS.xlam'!dsfunnew(C1)";
            wb2.Worksheets[0].Copy(sheet);
            Console.WriteLine("After copy: " + wb2.Worksheets[0].Cells[0, 0].Formula);
        }
    }
}
```

### See Also

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


