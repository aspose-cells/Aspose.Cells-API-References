---
title: MarkdownSaveOptions.SplitTablesByBlankRow
second_title: Aspose.Cells for .NET API Reference
description: MarkdownSaveOptions property. Indicates whether blank rows in the worksheet should be treated as table separators when exporting to Markdown. The default value is false
type: docs
url: /net/aspose.cells/markdownsaveoptions/splittablesbyblankrow/
---
## MarkdownSaveOptions.SplitTablesByBlankRow property

Indicates whether blank rows in the worksheet should be treated as table separators when exporting to Markdown. The default value is false.

```csharp
public bool SplitTablesByBlankRow { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertySplitTablesByBlankRowDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data with blank rows to demonstrate table splitting
            worksheet.Cells["A1"].Value = "Table 1 Header";
            worksheet.Cells["B1"].Value = "Value 1";
            worksheet.Cells["A2"].Value = "Data 1";
            worksheet.Cells["B2"].Value = "Data 2";

            // Add a blank row (row 3)
            worksheet.Cells["A4"].Value = "Table 2 Header";
            worksheet.Cells["B4"].Value = "Value 2";
            worksheet.Cells["A5"].Value = "Data 3";
            worksheet.Cells["B5"].Value = "Data 4";

            // Create MarkdownSaveOptions instance
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Display the default SplitTablesByBlankRow value
                Console.WriteLine("Default SplitTablesByBlankRow value: " +
                    saveOptions.SplitTablesByBlankRow);

                // Set SplitTablesByBlankRow to true to split tables by blank rows
                saveOptions.SplitTablesByBlankRow = true;

                // Display the updated value
                Console.WriteLine("Updated SplitTablesByBlankRow value: " +
                    saveOptions.SplitTablesByBlankRow);

                // Save the workbook as markdown with table splitting enabled
                workbook.Save("SplitTablesByBlankRowDemo.md", saveOptions);
                Console.WriteLine("Markdown file saved with table splitting by blank rows enabled.");
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


