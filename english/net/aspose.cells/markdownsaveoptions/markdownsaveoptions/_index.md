---
title: MarkdownSaveOptions.MarkdownSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: MarkdownSaveOptions constructor. Creates options for saving markdown document
type: docs
url: /net/aspose.cells/markdownsaveoptions/markdownsaveoptions/
---
## MarkdownSaveOptions constructor

Creates options for saving markdown document

```csharp
public MarkdownSaveOptions()
```

### Examples

```csharp
// Called: MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
public static void MarkdownSaveOptions_Constructor()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Hello&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;World&quot;);

            // Create an instance of MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                Encoding = Encoding.UTF8,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                LineSeparator = &quot;\n&quot;,
                ClearData = false,
                CachedFileFolder = &quot;C:\\Temp&quot;,
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = false,
                SortExternalNames = false,
                RefreshChartCache = false,
                UpdateSmartArt = false
            };

            // Save the workbook as a Markdown file
            workbook.Save(&quot;MarkdownSaveOptionsExample.md&quot;, saveOptions);

            Console.WriteLine(&quot;Workbook saved as Markdown file successfully.&quot;);
        }
```

### See Also

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


