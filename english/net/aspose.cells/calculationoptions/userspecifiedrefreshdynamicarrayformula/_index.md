---
title: CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula
second_title: Aspose.Cells for .NET API Reference
description: CalculationOptions property. Indicates whether user has explicitly specified the behavior of refreshing dynamic array formulas before calculating specified formulas
type: docs
url: /net/aspose.cells/calculationoptions/userspecifiedrefreshdynamicarrayformula/
---
## CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula property

Indicates whether user has explicitly specified the behavior of refreshing dynamic array formulas before calculating specified formulas.

```csharp
public bool UserSpecifiedRefreshDynamicArrayFormula { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationOptionsPropertyUserSpecifiedRefreshDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Create a sample worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to make the example meaningful
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Create CalculationOptions instance
                CalculationOptions options = new CalculationOptions();

                // Display the current value of the UserSpecifiedRefreshDynamicArrayFormula property
                Console.WriteLine("UserSpecifiedRefreshDynamicArrayFormula value: " +
                    options.UserSpecifiedRefreshDynamicArrayFormula);

                // Show how the property affects behavior
                Console.WriteLine("UserSpecifiedRefreshDynamicArrayFormula has been demonstrated");

                // Save the result
                workbook.Save("UserSpecifiedRefreshDynamicArrayFormulaDemo.xlsx");
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


