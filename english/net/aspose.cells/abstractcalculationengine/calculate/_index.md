---
title: AbstractCalculationEngine.Calculate
second_title: Aspose.Cells for .NET API Reference
description: AbstractCalculationEngine method. Calculates one function with given data
type: docs
url: /net/aspose.cells/abstractcalculationengine/calculate/
---
## AbstractCalculationEngine.Calculate method

Calculates one function with given data.

```csharp
public abstract void Calculate(CalculationData data)
```

| Parameter | Type | Description |
| --- | --- | --- |
| data | CalculationData | the required data to calculate function such as function name, parameters, ...etc. |

### Remarks

User should set the calculated value for given data for all functions(including excel native functions) that he wants to calculate by himself in this implementation.

### Examples

```csharp
namespace AsposeCellsExamples.AbstractCalculationEngineMethodCalculateWithCalculationDataDemo
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEngineMethodCalculateWithCalculationDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(3);
            worksheet.Cells["A3"].Formula = "=CUSTOMSUM(A1,A2)";
            
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalculationEngine();
            
            try
            {
                workbook.CalculateFormula(options);
                Console.WriteLine("Custom calculation result: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Calculate method: {ex.Message}");
            }
            
            workbook.Save("AbstractCalculationEngineDemo.xlsx");
        }

        class CustomCalculationEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName.ToUpper() == "CUSTOMSUM")
                {
                    if (data.ParamCount == 2)
                    {
                        try
                        {
                            double val1 = Convert.ToDouble(data.GetParamValue(0));
                            double val2 = Convert.ToDouble(data.GetParamValue(1));
                            data.CalculatedValue = $"Sum: {val1 + val2}";
                        }
                        catch
                        {
                            data.CalculatedValue = "#VALUE!";
                        }
                    }
                }
            }
        }
    }
}
```

### See Also

* class [CalculationData](../../calculationdata/)
* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


