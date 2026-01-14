---
title: MarkdownSaveOptions.CalculateFormula
second_title: Aspose.Cells for .NET API Reference
description: MarkdownSaveOptions property. Indicates whether to calculate formulas before saving markdown file
type: docs
url: /net/aspose.cells/markdownsaveoptions/calculateformula/
---
## MarkdownSaveOptions.CalculateFormula property

Indicates whether to calculate formulas before saving markdown file.

```csharp
public bool CalculateFormula { get; set; }
```

### Remarks

The default value is false.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data with formulas
            worksheet.Cells["A1"].PutValue("Price");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["C1"].PutValue("Total");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["C2"].Formula = "=A2*B2";

            try
            {
                // Create MarkdownSaveOptions instance
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Display the default value of CalculateFormula
                Console.WriteLine("Default CalculateFormula value: " + saveOptions.CalculateFormula);

                // Set CalculateFormula to true to calculate formulas before saving
                saveOptions.CalculateFormula = true;
                Console.WriteLine("CalculateFormula set to: " + saveOptions.CalculateFormula);

                // Save the workbook with formula calculation enabled
                workbook.Save("CalculateFormula_Enabled.md", saveOptions);

                // Set CalculateFormula to false to save formulas as-is
                saveOptions.CalculateFormula = false;
                Console.WriteLine("CalculateFormula set to: " + saveOptions.CalculateFormula);

                // Save the workbook with formula calculation disabled
                workbook.Save("CalculateFormula_Disabled.md", saveOptions);

                Console.WriteLine("CalculateFormula demonstration completed successfully.");
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

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


