---
title: CalculationData.GetParamValueInArrayMode
second_title: Aspose.Cells for .NET API Reference
description: CalculationData method. Gets the values of the parameter at a given index. If the parameter is some kind of expression that needs to be calculated then it will be calculated in array mode
type: docs
url: /net/aspose.cells/calculationdata/getparamvalueinarraymode/
---
## CalculationData.GetParamValueInArrayMode method

Gets the value(s) of the parameter at a given index. If the parameter is some kind of expression that needs to be calculated, then it will be calculated in array mode.

```csharp
public object[][] GetParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index of the parameter(0 based) |
| maxRowCount | Int32 | The row count limit for the returned array. If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | Int32 | The column count limit for the returned array. If it is non-positive or greater than the actual row count, then actual column count will be used. |

### Return Value

An array which contains all items represented by the specified parameter.

### Remarks

For an expression that needs to be calculated, taking A:A+B:B as an example: In value mode it will be calculated to a single value according to current cell base. But in array mode, all values of A1+B1,A2+B2,A3+B3,... will be calculated and used to construct the returned array. And for such kind of situation, it is better to specify the limit for the row/column count (such as according to [`MaxDataRow`](../../cells/maxdatarow/) and [`MaxDataColumn`](../../cells/maxdatacolumn/)), otherwise the returned large array may increase memory cost with large amount of useless data.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataMethodGetParamValueInArrayModeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for context
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Formula = "=SUM(A1:C3)";

            try
            {
                // Create calculation options with custom engine
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new ArrayModeCalculationEngine();
                workbook.CalculateFormula(options);

                Console.WriteLine("GetParamValueInArrayMode method called successfully");
                workbook.Save("GetParamValueInArrayModeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetParamValueInArrayMode: {ex.Message}");
            }
        }

        private class ArrayModeCalculationEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName == "SUM")
                {
                    // Call GetParamValueInArrayMode with realistic parameters
                    object[][] paramArray = data.GetParamValueInArrayMode(0, 5, 3);

                    Console.WriteLine($"Parameter array dimensions: {paramArray.Length} rows");
                    if (paramArray.Length > 0)
                    {
                        Console.WriteLine($"First row has {paramArray[0].Length} columns");
                    }
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


