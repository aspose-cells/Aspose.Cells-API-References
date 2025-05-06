---
title: CalculationOptions.CalcStackSize
second_title: Aspose.Cells for .NET API Reference
description: CalculationOptions property. The stack size for calculating cells recursively. Default value is 200
type: docs
url: /net/aspose.cells/calculationoptions/calcstacksize/
---
## CalculationOptions.CalcStackSize property

The stack size for calculating cells recursively. Default value is 200.

```csharp
public int CalcStackSize { get; set; }
```

### Remarks

When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2.

### Examples

```csharp
// Called: CalcStackSize = 200,
public static void Property_CalcStackSize()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells[&quot;A1&quot;].PutValue(10.555);
            worksheet.Cells[&quot;A2&quot;].PutValue(20.6666);
            worksheet.Cells[&quot;A3&quot;].PutValue(30.7777);
            worksheet.Cells[&quot;A4&quot;].Formula = &quot;=SUM(A1:A3)&quot;;

            // Create an instance of CalculationOptions
            CalculationOptions calcOptions = new CalculationOptions
            {
                IgnoreError = true,
                Recursive = true,
                CalcStackSize = 200,
                PrecisionStrategy = CalculationPrecisionStrategy.Round,
                CharacterEncoding = Encoding.UTF8
            };

            // Optionally, you can set a custom calculation engine or monitor
            // calcOptions.CustomEngine = new MyCustomEngine();
            // calcOptions.CalculationMonitor = new MyCalculationMonitor();

            // Calculate formulas in the workbook with the specified options
            workbook.CalculateFormula(calcOptions);

            // Save the workbook
            workbook.Save(&quot;CalculationOptionsExample.xlsx&quot;);
            workbook.Save(&quot;CalculationOptionsExample.pdf&quot;);

        }
```

### See Also

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


