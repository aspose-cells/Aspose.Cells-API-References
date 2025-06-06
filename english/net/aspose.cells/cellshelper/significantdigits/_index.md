---
title: CellsHelper.SignificantDigits
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper property. Gets and sets the number of significant digits. The default value is 17
type: docs
url: /net/aspose.cells/cellshelper/significantdigits/
---
## CellsHelper.SignificantDigits property

Gets and sets the number of significant digits. The default value is 17.

```csharp
public static int SignificantDigits { get; set; }
```

### Remarks

Only could be 15 or 17 now.

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertySignificantDigitsDemo
    {
        public static void Run()
        {
            // Set significant digits
            CellsHelper.SignificantDigits = 15;
            
            // Demonstrate the property usage
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
            
            // Create a workbook to demonstrate significant digits in calculations
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Set values that will be affected by significant digits
            worksheet.Cells["A1"].PutValue(1.2345678912345678);
            worksheet.Cells["A2"].PutValue(1.2345678912345678);
            worksheet.Cells["A3"].Formula = "=A1+A2";
            
            // Calculate formulas with the set significant digits
            workbook.CalculateFormula();
            
            // Output the results
            Console.WriteLine("Value with significant digits: " + worksheet.Cells["A3"].Value);
        }
    }
}
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


