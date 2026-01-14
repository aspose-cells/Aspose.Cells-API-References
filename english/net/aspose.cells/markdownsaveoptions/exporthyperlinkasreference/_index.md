---
title: MarkdownSaveOptions.ExportHyperlinkAsReference
second_title: Aspose.Cells for .NET API Reference
description: MarkdownSaveOptions property. Indicates whether to export hyperlink using reference definitions instead of inline format. The default value is false
type: docs
url: /net/aspose.cells/markdownsaveoptions/exporthyperlinkasreference/
---
## MarkdownSaveOptions.ExportHyperlinkAsReference property

Indicates whether to export hyperlink using reference definitions instead of inline format. The default value is false.

```csharp
public bool ExportHyperlinkAsReference { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyExportHyperlinkAsReferenceDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Put a sample text into a cell
            sheet.Cells["A1"].PutValue("Visit Aspose");

            // Add a hyperlink to the cell (A1)
            // Parameters: firstRow, firstColumn, totalRows, totalColumns, hyperlink
            sheet.Hyperlinks.Add(0, 0, 1, 1, "https://www.aspose.com");

            // Initialize Markdown save options
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Directly access the ExportHyperlinkAsReference property (read‑only in this demo)
                Console.WriteLine("ExportHyperlinkAsReference value: " + saveOptions.ExportHyperlinkAsReference);

                // Save the workbook as markdown; the property (if true) will affect how hyperlinks are exported
                workbook.Save("ExportHyperlinkAsReferenceDemo.md", saveOptions);
                Console.WriteLine("Workbook saved as markdown.");
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


