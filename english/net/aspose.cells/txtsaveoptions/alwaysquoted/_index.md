---
title: TxtSaveOptions.AlwaysQuoted
second_title: Aspose.Cells for .NET API Reference
description: TxtSaveOptions property. Indicates whether always adding  for each field. If true then all values will be quoted If false then values will only be quoted when neededfor example when values contain special characters such as   n or separator character. Default is false
type: docs
url: /net/aspose.cells/txtsaveoptions/alwaysquoted/
---
## TxtSaveOptions.AlwaysQuoted property

Indicates whether always adding '"' for each field. If true then all values will be quoted; If false then values will only be quoted when needed(for example, when values contain special characters such as '"' , '\n' or separator character). Default is false.

```csharp
[Obsolete("Use QuoteType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AlwaysQuoted { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use QuoteType property instead. This property will be removed 12 months later since August 2012. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: AlwaysQuoted = false,
public static void Property_AlwaysQuoted()
        {
            // Create a workbook with some data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Name&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Age&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;John Doe&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(30);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;Jane Smith&quot;);
            worksheet.Cells[&quot;B3&quot;].PutValue(25);

            // Create TxtSaveOptions object and set properties
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = &apos;,&apos;,
                SeparatorString = &quot;,&quot;,
                Encoding = Encoding.UTF8,
                AlwaysQuoted = false,
                QuoteType = TxtValueQuoteType.Normal,
                FormatStrategy = CellValueFormatStrategy.DisplayStyle,
                TrimLeadingBlankRowAndColumn = true,
                TrimTailingBlankCells = false,
                KeepSeparatorsForBlankRow = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
                ExportQuotePrefix = false,
                ExportAllSheets = false,
                ClearData = false,
                CachedFileFolder = &quot;cache&quot;,
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };

            // Save the workbook as a text file with the specified options
            workbook.Save(&quot;TxtSaveOptionsExample.txt&quot;, saveOptions);

            Console.WriteLine(&quot;Workbook saved successfully with TxtSaveOptions.&quot;);
        }
```

### See Also

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


