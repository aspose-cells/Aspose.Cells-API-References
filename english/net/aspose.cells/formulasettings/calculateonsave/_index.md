---
title: FormulaSettings.CalculateOnSave
second_title: Aspose.Cells for .NET API Reference
description: FormulaSettings property. Indicates whether to recalculate the workbook before saving the document when in manual calculation mode
type: docs
url: /net/aspose.cells/formulasettings/calculateonsave/
---
## FormulaSettings.CalculateOnSave property

Indicates whether to recalculate the workbook before saving the document, when in manual calculation mode.

```csharp
public bool CalculateOnSave { get; set; }
```

### Remarks

This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculateOnSaveDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the worksheet and add some data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Disable CalculateOnSave (default is false)
            workbook.Settings.FormulaSettings.CalculateOnSave = false;
            
            // Save without calculating formulas
            workbook.Save("output_without_calculation.xlsx");

            // Enable CalculateOnSave
            workbook.Settings.FormulaSettings.CalculateOnSave = true;
            
            // Save with formula calculation
            workbook.Save("output_with_calculation.xlsx");
        }
    }
}
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


