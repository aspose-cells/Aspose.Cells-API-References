---
title: CalculationData.Worksheet
second_title: Aspose.Cells for .NET API Reference
description: CalculationData property. Gets the Worksheet object where the function is
type: docs
url: /net/aspose.cells/calculationdata/worksheet/
---
## CalculationData.Worksheet property

Gets the Worksheet object where the function is.

```csharp
public Worksheet Worksheet { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyWorksheetDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Add some data to make the example meaningful
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

                // Create calculation options with custom engine
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new WorksheetDemoEngine();

                // Calculate formulas with options
                workbook.CalculateFormula(options);

                // Display the result
                Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);

                // Save the result
                workbook.Save("WorksheetDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class WorksheetDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                // Access the read-only Worksheet property
                Worksheet worksheet = data.Worksheet;
                Console.WriteLine($"Function is in worksheet: {worksheet.Name}");

                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object arg = data.GetParamValue(i);
                    if (arg is double)
                    {
                        sum += (double)arg;
                    }
                }
                data.CalculatedValue = sum;
            }
        }
    }
}
```

### See Also

* class [Worksheet](../../worksheet/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


