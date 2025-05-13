---
title: CalculationOptions.PrecisionStrategy
second_title: Aspose.Cells for .NET API Reference
description: CalculationOptions property. Specifies the strategy for processing precision of calculation
type: docs
url: /net/aspose.cells/calculationoptions/precisionstrategy/
---
## CalculationOptions.PrecisionStrategy property

Specifies the strategy for processing precision of calculation.

```csharp
public CalculationPrecisionStrategy PrecisionStrategy { get; set; }
```

### Examples

```csharp
// Called: PrecisionStrategy = CalculationPrecisionStrategy.Round,
public static void CalculationOptions_Property_PrecisionStrategy()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells["A1"].PutValue(10.555);
            worksheet.Cells["A2"].PutValue(20.6666);
            worksheet.Cells["A3"].PutValue(30.7777);
            worksheet.Cells["A4"].Formula = "=SUM(A1:A3)";

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
            workbook.Save("CalculationOptionsExample.xlsx");
            workbook.Save("CalculationOptionsExample.pdf");

        }
```

### See Also

* enum [CalculationPrecisionStrategy](../../calculationprecisionstrategy/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


