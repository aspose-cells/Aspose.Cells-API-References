---
title: Class CalculationData
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.CalculationData class. Represents the required data when calculating one function such as function name parameters ...etc
type: docs
url: /net/aspose.cells/calculationdata/
---
## CalculationData class

Represents the required data when calculating one function, such as function name, parameters, ...etc.

```csharp
public class CalculationData
```

## Properties

| Name | Description |
| --- | --- |
| [CalculatedValue](../../aspose.cells/calculationdata/calculatedvalue/) { get; set; } | Gets or sets the calculated value for this function. |
| [Cell](../../aspose.cells/calculationdata/cell/) { get; } | Gets the Cell object where the function is. |
| [CellColumn](../../aspose.cells/calculationdata/cellcolumn/) { get; } | Gets the column index of the cell where the function is. |
| [CellRow](../../aspose.cells/calculationdata/cellrow/) { get; } | Gets the row index of the cell where the function is. |
| [FunctionName](../../aspose.cells/calculationdata/functionname/) { get; } | Gets the function name to be calculated. |
| [ParamCount](../../aspose.cells/calculationdata/paramcount/) { get; } | Gets the count of parameters |
| [Workbook](../../aspose.cells/calculationdata/workbook/) { get; } | Gets the Workbook object where the function is. |
| [Worksheet](../../aspose.cells/calculationdata/worksheet/) { get; } | Gets the Worksheet object where the function is. |

## Methods

| Name | Description |
| --- | --- |
| [GetParamText](../../aspose.cells/calculationdata/getparamtext/)(int) | Gets the literal text of the parameter at the given index. |
| [GetParamValue](../../aspose.cells/calculationdata/getparamvalue/)(int) | Gets the represented value object of the parameter at a given index. |
| [GetParamValueInArrayMode](../../aspose.cells/calculationdata/getparamvalueinarraymode/)(int, int, int) | Gets the value(s) of the parameter at a given index. If the parameter is some kind of expression that needs to be calculated, then it will be calculated in array mode. |

### Remarks

All objects provided by this class are for "read" purpose only. User should not change any data in the Workbook during the formula calculation process, Otherwise unexpected result or Exception may be caused.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCalculationDataDemo
    {
        public static void Run()
        {
            try
            {
                // Prepare a simple workbook and worksheet
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Name = "DemoSheet";

                // Put some values that will be used as parameters in a custom function
                sheet.Cells["A1"].PutValue(5);
                sheet.Cells["A2"].PutValue(10);

                // Set a formula that invokes the custom function
                sheet.Cells["B1"].Formula = "=MYFUNC(A1, A2)";

                // Configure calculation options to use a custom engine
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new DemoEngine();

                // Perform calculation – the custom engine will receive a CalculationData instance
                workbook.CalculateFormula(options);

                // Output the result of the custom function
                Console.WriteLine("Custom function result (B1): " + sheet.Cells["B1"].Value);

                // Save the workbook for completeness
                workbook.Save("CalculationDataDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with CalculationData: {ex.Message}");
            }
        }

        // Custom calculation engine that demonstrates accessing CalculationData members
        private class DemoEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                // Ensure we are handling the expected custom function
                if (data.FunctionName != null &&
                    data.FunctionName.Equals("MYFUNC", StringComparison.OrdinalIgnoreCase))
                {
                    // Retrieve parameter values (they are returned as objects)
                    object param0 = data.GetParamValue(0);
                    object param1 = data.GetParamValue(1);

                    // Convert parameters to double for calculation
                    double val0 = Convert.ToDouble(param0);
                    double val1 = Convert.ToDouble(param1);
                    double result = val0 + val1; // simple addition

                    // Assign the calculated result
                    data.CalculatedValue = result;

                    // Demonstrate reading read‑only properties
                    Console.WriteLine("[Engine] FunctionName : " + data.FunctionName);
                    Console.WriteLine("[Engine] ParamCount   : " + data.ParamCount);
                    Console.WriteLine("[Engine] CellRow      : " + data.CellRow);
                    Console.WriteLine("[Engine] CellColumn   : " + data.CellColumn);
                }
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


