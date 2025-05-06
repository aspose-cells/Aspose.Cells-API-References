---
title: TxtSaveOptions.ExportArea
second_title: Aspose.Cells for .NET API Reference
description: TxtSaveOptions property. The range of cells to be exported
type: docs
url: /net/aspose.cells/txtsaveoptions/exportarea/
---
## TxtSaveOptions.ExportArea property

The range of cells to be exported.

```csharp
public CellArea ExportArea { get; set; }
```

### Remarks

If the exported area has been specified, [`TrimLeadingBlankRowAndColumn`](../trimleadingblankrowandcolumn/) will takes no effect.

### Examples

```csharp
// Called: ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
public static void Property_ExportArea()
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

* struct [CellArea](../../cellarea/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


