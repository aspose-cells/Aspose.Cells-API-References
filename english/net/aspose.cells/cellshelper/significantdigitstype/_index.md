---
title: CellsHelper.SignificantDigitsType
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper property. Gets and sets the default type of significant digits for outputing numeric values. Default value is G17
type: docs
url: /net/aspose.cells/cellshelper/significantdigitstype/
---
## CellsHelper.SignificantDigitsType property

Gets and sets the default type of significant digits for outputing numeric values. Default value is G17.

```csharp
public static SignificantDigitsType SignificantDigitsType { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperPropertySignificantDigitsTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Display the current SignificantDigitsType value
                Console.WriteLine("Current SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Set a new SignificantDigitsType value
                CellsHelper.SignificantDigitsType = SignificantDigitsType.G17;
                Console.WriteLine("Updated SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Create a workbook to demonstrate the effect
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Add a numeric value that will be affected by significant digits
                worksheet.Cells["A1"].PutValue(1.2345678912345678);
                worksheet.Cells["A2"].PutValue(1.2345678912345678);
                worksheet.Cells["A3"].Formula = "=A1+A2";

                // Calculate formulas with the current significant digits type
                workbook.CalculateFormula();

                // Display the result
                Console.WriteLine("Calculation result: " + worksheet.Cells["A3"].Value);

                // Change to another significant digits type
                CellsHelper.SignificantDigitsType = SignificantDigitsType.Rounding17;
                Console.WriteLine("Changed SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Recalculate with the new significant digits type
                workbook.CalculateFormula();
                Console.WriteLine("Recalculated result: " + worksheet.Cells["A3"].Value);

                // Save the workbook
                workbook.Save("SignificantDigitsTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [SignificantDigitsType](../../significantdigitstype/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


