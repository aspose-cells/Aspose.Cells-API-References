---
title: CalculationData.GetParamValueInArrayMode
second_title: Aspose.Cells for .NET API Reference
description: CalculationData method. Gets the values of the parameter at given index. If the parameter is some kind of expression that needs to be calculated then it will be calculated in array mode
type: docs
url: /net/aspose.cells/calculationdata/getparamvalueinarraymode/
---
## CalculationData.GetParamValueInArrayMode method

Gets the value(s) of the parameter at given index. If the parameter is some kind of expression that needs to be calculated, then it will be calculated in array mode.

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
using System;

namespace AsposeCellsExamples
{
    public class CalculationDataMethodGetParamValueInArrayModeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Create sample data for demonstration
            object[][] sampleArray = new object[][]
            {
                new object[] { 1.0, 2.0, 3.0 },
                new object[] { 4.0, 5.0, 6.0 },
                new object[] { 7.0, 8.0, 9.0 }
            };

            // Create a mock CalculationData class for demonstration
            CalculationDataMock data = new CalculationDataMock(sampleArray);

            // Demonstrate GetParamValueInArrayMode with (0, 3, 3) parameters
            object[][] result = data.GetParamValueInArrayMode(0, 3, 3);

            // Calculate and display the sum of all values
            double sum = 0;
            for (int i = 0; i < result.Length; i++)
            {
                for (int j = 0; j < result[i].Length; j++)
                {
                    sum += (double)result[i][j];
                }
            }
            Console.WriteLine("Sum of all array values: " + sum);
        }
    }

    // Mock CalculationData class for demonstration
    public class CalculationDataMock
    {
        private object[][] _arrayData;

        public CalculationDataMock(object[][] arrayData)
        {
            _arrayData = arrayData;
        }

        public object[][] GetParamValueInArrayMode(int paramIndex, int rowCount, int columnCount)
        {
            // In a real implementation, this would retrieve the array data based on parameters
            // For demo, we just return our sample data
            return _arrayData;
        }
    }
}
```

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


