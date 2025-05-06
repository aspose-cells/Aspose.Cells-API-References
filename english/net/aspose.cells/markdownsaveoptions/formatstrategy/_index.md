---
title: MarkdownSaveOptions.FormatStrategy
second_title: Aspose.Cells for .NET API Reference
description: MarkdownSaveOptions property. Gets and sets the format strategy when exporting the cell value as string
type: docs
url: /net/aspose.cells/markdownsaveoptions/formatstrategy/
---
## MarkdownSaveOptions.FormatStrategy property

Gets and sets the format strategy when exporting the cell value as string.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Examples

```csharp
// Called: FormatStrategy = CellValueFormatStrategy.DisplayString,
public static void Property_FormatStrategy()
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

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


