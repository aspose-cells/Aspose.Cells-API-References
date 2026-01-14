---
title: CalculationOptions.RefreshDynamicArrayFormula
second_title: Aspose.Cells for .NET API Reference
description: CalculationOptions property. Indicates whether dynamic array formulas should be refreshed before calculating formulas
type: docs
url: /net/aspose.cells/calculationoptions/refreshdynamicarrayformula/
---
## CalculationOptions.RefreshDynamicArrayFormula property

Indicates whether dynamic array formulas should be refreshed before calculating formulas.

```csharp
public bool RefreshDynamicArrayFormula { get; set; }
```

### Remarks

If this property has been specified explicitly, then the specified value will be used to determine whether refresh dynamic array formulas. Otherwise([`UserSpecifiedRefreshDynamicArrayFormula`](../userspecifiedrefreshdynamicarrayformula/) is flase), the default value of it depends on what kind of formulas need to be calculated: For calculating formulas for the workbook, such as [`CalculateFormula`](../../workbook/calculateformula/), this property will be taken as true. For other cases, such as [`Calculate`](../../cell/calculate/) or [`CalculateFormula`](../../worksheet/calculateformula/), this property will be taken as false.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationOptionsPropertyRefreshDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a dynamic array formula to demonstrate the functionality
            worksheet.Cells["A1"].Value = 1;
            worksheet.Cells["A2"].Value = 2;
            worksheet.Cells["A3"].Value = 3;
            worksheet.Cells["B1"].Formula = "=A1:A3"; // Dynamic array formula

            // Create CalculationOptions instance
            CalculationOptions options = new CalculationOptions();

            try
            {
                // Display the default value of RefreshDynamicArrayFormula
                Console.WriteLine("Default RefreshDynamicArrayFormula value: " + options.RefreshDynamicArrayFormula);

                // Set the property to true to refresh dynamic array formulas
                options.RefreshDynamicArrayFormula = true;
                Console.WriteLine("After setting to true: " + options.RefreshDynamicArrayFormula);

                // Calculate formulas with the specified options
                workbook.CalculateFormula(options);

                // Display the calculated result
                Console.WriteLine("Dynamic array formula result: " + worksheet.Cells["B1"].Value);

                // Save the workbook
                workbook.Save("RefreshDynamicArrayFormulaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


