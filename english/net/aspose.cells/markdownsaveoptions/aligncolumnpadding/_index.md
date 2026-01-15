---
title: MarkdownSaveOptions.AlignColumnPadding
second_title: Aspose.Cells for .NET API Reference
description: MarkdownSaveOptions property. Indicates whether column alignment is enabled for generated Markdown tables. When enabled columns are aligned by padding cell content with the specified charactertypically   for spaces. Set to 0 to disable column alignment default
type: docs
url: /net/aspose.cells/markdownsaveoptions/aligncolumnpadding/
---
## MarkdownSaveOptions.AlignColumnPadding property

Indicates whether column alignment is enabled for generated Markdown tables. When enabled, columns are aligned by padding cell content with the specified character(typically ' ' for spaces). Set to '\0' to disable column alignment (default).

```csharp
public char AlignColumnPadding { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyAlignColumnPaddingDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to demonstrate column alignment
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = "1.99";
            worksheet.Cells["C2"].Value = "10";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B3"].Value = "0.99";
            worksheet.Cells["C3"].Value = "20";

            // Create MarkdownSaveOptions instance
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Display the default AlignColumnPadding value
                Console.WriteLine("Default AlignColumnPadding value: '" +
                    saveOptions.AlignColumnPadding + "'");

                // Set AlignColumnPadding to space character for column alignment
                saveOptions.AlignColumnPadding = ' ';

                // Display the updated value
                Console.WriteLine("Updated AlignColumnPadding value: '" +
                    saveOptions.AlignColumnPadding + "'");

                // Save the workbook as markdown with column alignment
                workbook.Save("AlignColumnPaddingDemo.md", saveOptions);
                Console.WriteLine("Markdown file saved with column alignment enabled.");
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


