---
title: CalculationData.ParamCount
second_title: Aspose.Cells for .NET API Reference
description: CalculationData property. Gets the count of parameters
type: docs
url: /net/aspose.cells/calculationdata/paramcount/
---
## CalculationData.ParamCount property

Gets the count of parameters

```csharp
public int ParamCount { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyParamCountDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook and get the first worksheet
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Populate some cells that will be used as parameters
                sheet.Cells["A1"].PutValue(10);
                sheet.Cells["A2"].PutValue(20);
                sheet.Cells["A3"].PutValue(30);

                // Set a formula that calls a custom function with three arguments
                sheet.Cells["B1"].Formula = "=DEMOPARAM(A1, A2, A3)";

                // Configure calculation options to use a custom engine
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new ParamCountEngine();

                // Perform calculation
                workbook.CalculateFormula(options);

                // The custom engine returns the ParamCount as the calculated value
                Console.WriteLine("ParamCount reported by custom function: " + sheet.Cells["B1"].Value);
                
                // Optionally save the workbook
                workbook.Save("ParamCountDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Custom calculation engine that demonstrates reading the ParamCount property
        private class ParamCountEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                // Identify the custom function by name
                if (data.FunctionName != null && data.FunctionName.Equals("DEMOPARAM", StringComparison.OrdinalIgnoreCase))
                {
                    // Read the read‑only ParamCount property
                    int count = data.ParamCount;

                    // Use the count as the result of the function
                    data.CalculatedValue = count;
                }
            }
        }
    }
}
```

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


