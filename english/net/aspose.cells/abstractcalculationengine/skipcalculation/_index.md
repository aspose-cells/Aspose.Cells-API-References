---
title: AbstractCalculationEngine.SkipCalculation
second_title: Aspose.Cells for .NET API Reference
description: AbstractCalculationEngine method. Skips the calculation for the entire formula that references the function currently under evaluation
type: docs
url: /net/aspose.cells/abstractcalculationengine/skipcalculation/
---
## AbstractCalculationEngine.SkipCalculation method

Skips the calculation for the entire formula that references the function currently under evaluation.

```csharp
public void SkipCalculation()
```

### Remarks

This method can be invoked in the implementation of [`Calculate`](../calculate/) to skip the calculation for the entire formula and the original value of the formula will be kept without change.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEngineMethodSkipCalculationDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data for context
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Formula = "=SKIPFUNC(A1,A2)";

            // Create custom calculation engine
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomSkipEngine();

            try
            {
                // Calculate the workbook which will trigger our custom engine
                workbook.CalculateFormula(options);

                // Display the result (should be skipped)
                Console.WriteLine("Calculation result: " + worksheet.Cells["A3"].StringValue);

                // Save the workbook
                workbook.Save("SkipCalculationDemo.xlsx");
                Console.WriteLine("SkipCalculation method demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating SkipCalculation: {ex.Message}");
            }
        }
    }

    public class CustomSkipEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName.ToUpper() == "SKIPFUNC")
            {
                // Skip the calculation for this formula
                SkipCalculation();
                data.CalculatedValue = "#SKIPPED!";
            }
        }
    }
}
```

### See Also

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


