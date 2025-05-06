---
title: MarkdownSaveOptions.LineSeparator
second_title: Aspose.Cells for .NET API Reference
description: MarkdownSaveOptions property. Gets and sets the line separator
type: docs
url: /net/aspose.cells/markdownsaveoptions/lineseparator/
---
## MarkdownSaveOptions.LineSeparator property

Gets and sets the line separator.

```csharp
public string LineSeparator { get; set; }
```

### Examples

```csharp
// Called: LineSeparator = &amp;quot;\n&amp;quot;,
public static void Property_LineSeparator()
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


