---
title: MarkdownLoadOptions.HasFormula
second_title: Aspose.Cells for .NET API Reference
description: MarkdownLoadOptions property. Indicates whether the text is formula if it starts with 
type: docs
url: /net/aspose.cells/markdownloadoptions/hasformula/
---
## MarkdownLoadOptions.HasFormula property

Indicates whether the text is formula if it starts with "=".

```csharp
public bool HasFormula { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // Create an instance of MarkdownLoadOptions
                MarkdownLoadOptions options = new MarkdownLoadOptions();

                // Display the default value of HasFormula
                Console.WriteLine($"Default HasFormula value: {options.HasFormula}");

                // Set HasFormula to true
                options.HasFormula = true;
                Console.WriteLine($"HasFormula set to: {options.HasFormula}");

                // Set HasFormula to false
                options.HasFormula = false;
                Console.WriteLine($"HasFormula set to: {options.HasFormula}");

                // Create a workbook with sample markdown content
                Workbook workbook = new Workbook();

                // Save the workbook to demonstrate the options can be used
                workbook.Save("HasFormulaDemo.xlsx");

                Console.WriteLine("HasFormula property demonstration completed successfully.");
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

* class [MarkdownLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


