---
title: SplitPartInfo.PartIndex
second_title: Aspose.Cells for .NET API Reference
description: SplitPartInfo property. Index of current part in sequence0 based. 1 means there are no multiple parts so the result is single
type: docs
url: /net/aspose.cells.lowcode/splitpartinfo/partindex/
---
## SplitPartInfo.PartIndex property

Index of current part in sequence(0 based). -1 means there are no multiple parts so the result is single.

```csharp
public int PartIndex { get; }
```

### Remarks

If multiple sheets need to be processed and every sheet is processed(split) separately, the part index always starts from 0 for every sheet. For example, when converting workbook to images, it represents the output page index of currently processed sheet. And -1 denotes there is only one page for current sheet.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SplitPartInfoPropertyPartIndexDemo
    {
        public static void Run()
        {
            try
            {
                // Create a workbook with multiple sheets
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Worksheets.Add("Sheet2");
                workbook.Worksheets.Add("Sheet3");

                // Save the workbook to use with split operation
                workbook.Save("sample.xlsx");

                // Create load options
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                loadOptions.InputFile = "sample.xlsx";

                // Create split options with custom provider
                LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
                splitOptions.LoadOptions = loadOptions;
                splitOptions.SaveOptionsProvider = new CustomPartIndexProvider();

                // Process the split operation
                SpreadsheetSplitter.Process(splitOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomPartIndexProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Demonstrate reading the PartIndex property
            Console.WriteLine($"Current part PartIndex: {partInfo.PartIndex}");
            Console.WriteLine($"Current part SheetIndex: {partInfo.SheetIndex}");
            Console.WriteLine($"Current part SheetName: {partInfo.SheetName}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Part_{partInfo.PartIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### See Also

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


