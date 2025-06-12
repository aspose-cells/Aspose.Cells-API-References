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
using System;

namespace AsposeCellsExamples
{
    public class CalculationDataPropertyParamCountDemo
    {
        public static void Run()
        {
            // Create sample CalculationData with parameters
            CalculationData data = new CalculationData();
            
            // Add parameters to demonstrate ParamCount
            data.AddParamValue(10);  // Param 0
            data.AddParamValue(20);  // Param 1
            data.AddParamValue(30);  // Param 2
            data.AddParamValue(0);   // Param 3
            data.AddParamValue(1);   // Param 4
            data.AddParamValue(0);   // Param 5
            data.AddParamValue(1);   // Param 6 (optional 7th param)

            Console.WriteLine($"Parameter Count: {data.ParamCount}");

            // Demonstrate different behavior based on ParamCount
            if (data.ParamCount < 6)
            {
                Console.WriteLine("Error: Not enough parameters (need at least 6)");
                return;
            }

            if (data.ParamCount > 6)
            {
                Console.WriteLine("Using extended parameter set (7 parameters)");
                Console.WriteLine($"Interval: {data.GetParamValue(3)}");
                Console.WriteLine($"Headers: {data.GetParamValue(4)}");
            }
            else
            {
                Console.WriteLine("Using basic parameter set (6 parameters)");
                Console.WriteLine($"Interval: {data.GetParamValue(3)}");
            }

            // Sample calculation based on parameters
            int start = (int)data.GetParamValue(1);
            int end = (int)data.GetParamValue(2);
            int count = end - start + 1;
            
            if (data.ParamCount > 6)
            {
                count += 4; // Additional rows for extended params
            }

            Console.WriteLine($"Calculated row count: {count}");
        }
    }

    // Simplified CalculationData class for demonstration
    public class CalculationData
    {
        private object[] parameters = new object[10];
        private int paramCount = 0;

        public int ParamCount => paramCount;

        public void AddParamValue(object value)
        {
            if (paramCount < parameters.Length)
            {
                parameters[paramCount++] = value;
            }
        }

        public object GetParamValue(int index)
        {
            if (index >= 0 && index < paramCount)
            {
                return parameters[index];
            }
            return null;
        }
    }
}
```

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


