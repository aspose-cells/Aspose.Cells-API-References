---
title: FormulaSettings.EnableIterativeCalculation
second_title: Aspose.Cells for .NET API Reference
description: FormulaSettings property. Indicates whether to enable iterative calculation to resolve circular references
type: docs
url: /net/aspose.cells/formulasettings/enableiterativecalculation/
---
## FormulaSettings.EnableIterativeCalculation property

Indicates whether to enable iterative calculation to resolve circular references.

```csharp
public bool EnableIterativeCalculation { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyEnableIterativeCalculationDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Set up circular reference for demonstration
            worksheet.Cells["A1"].Formula = "=B1+1";
            worksheet.Cells["B1"].Formula = "=A1+1";
            
            // Enable iterative calculation with max iterations
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            workbook.Settings.FormulaSettings.MaxChange = 0.001;
            
            // Calculate formulas
            workbook.CalculateFormula();
            
            // Output results
            Console.WriteLine("A1 value after calculation: " + worksheet.Cells["A1"].DoubleValue);
            Console.WriteLine("B1 value after calculation: " + worksheet.Cells["B1"].DoubleValue);
        }
    }
}
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


