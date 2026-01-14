---
title: Class AbstractCalculationEngine
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.AbstractCalculationEngine class. Represents users custom calculation engine to extend the default calculation engine of Aspose.Cells
type: docs
url: /net/aspose.cells/abstractcalculationengine/
---
## AbstractCalculationEngine class

Represents user's custom calculation engine to extend the default calculation engine of Aspose.Cells.

```csharp
public abstract class AbstractCalculationEngine
```

## Properties

| Name | Description |
| --- | --- |
| virtual [IsParamArrayModeRequired](../../aspose.cells/abstractcalculationengine/isparamarraymoderequired/) { get; } | Indicates whether this engine needs the parameter to be calculated in array mode. Default value is false. If [`GetParamValueInArrayMode`](../calculationdata/getparamvalueinarraymode/) is required when calculating custom functions and user has not updated the definition for them (by [`UpdateCustomFunctionDefinition`](../workbook/updatecustomfunctiondefinition/)), this property needs to be set as true. |
| virtual [IsParamLiteralRequired](../../aspose.cells/abstractcalculationengine/isparamliteralrequired/) { get; } | Indicates whether this engine needs the literal text of the parameter while doing a calculation. Default value is false. |
| virtual [ProcessBuiltInFunctions](../../aspose.cells/abstractcalculationengine/processbuiltinfunctions/) { get; } | Whether built-in functions that have been supported by the built-in engine should be checked and processed by this implementation. Default is false. |

## Methods

| Name | Description |
| --- | --- |
| abstract [Calculate](../../aspose.cells/abstractcalculationengine/calculate/)(CalculationData) | Calculates one function with given data. |
| virtual [ForceRecalculate](../../aspose.cells/abstractcalculationengine/forcerecalculate/)(string) | Whether to force the given function to be recalculated always when calculating shared formulas. |
| [SkipCalculation](../../aspose.cells/abstractcalculationengine/skipcalculation/)() | Skips the calculation for the entire formula that references the function currently under evaluation. |

### Remarks

User should not modify any part of the Workbook directly in this implementation(except the calculated result of the custom function, which can be set by CalculationData.CalculatedValue property). Otherwise unexpected result or Exception may be caused. If user needs to change other data than calculated result in the implementation for some custom functions, for example, change cell's formula, style, ...etc., user should gather those data in this implementation and change them out of the scope of formula calculation.

### Examples

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // Example: Custom implementation for a function named "MYFUNC"
            if (data.FunctionName.ToUpper() == "MYFUNC")
            {
                // Assuming MYFUNC takes two parameters and returns their sum
                Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(0);
                Aspose.Cells.ReferredArea paramArea2 = (Aspose.Cells.ReferredArea)data.GetParamValue(1);

                double param1 = Convert.ToDouble(paramArea1.GetValue(0, 0));
                double param2 = Convert.ToDouble(paramArea2.GetValue(0, 0));
                data.CalculatedValue = param1 + param2;
            }
        }

        public override bool ForceRecalculate(string functionName)
        {
            // Force recalculation for custom function "MYFUNC"
            return functionName.ToUpper() == "MYFUNC";
        }
    }

    public class CalculationEngineDemo
    {
        public static void Test()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Put some values in cells
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);

            // Add a formula that uses the custom function
            sheet.Cells["A3"].Formula = "=MYFUNC(A1, A2)";

            // Set calculation options with the custom engine
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = new CustomCalculationEngine(),
                IgnoreError = false,
                Recursive = true
            };

            // Calculate formulas with custom engine
            workbook.CalculateFormula(options);

            // Print the result of the custom function
            Console.WriteLine("Result of MYFUNC(A1, A2): " + sheet.Cells["A3"].Value);

            // Save the workbook
            workbook.Save("CustomCalculationEngineExample.xlsx");
            workbook.Save("CustomCalculationEngineExample.pdf");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


