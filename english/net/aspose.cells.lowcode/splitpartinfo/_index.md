---
title: Class SplitPartInfo
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.LowCode.SplitPartInfo class. Represents the information of one input/output for multiple inputs/outputs such as current page to be rendered when converting spreadsheet to image
type: docs
url: /net/aspose.cells.lowcode/splitpartinfo/
---
## SplitPartInfo class

Represents the information of one input/output for multiple inputs/outputs, such as current page to be rendered when converting spreadsheet to image.

```csharp
public class SplitPartInfo
```

## Properties

| Name | Description |
| --- | --- |
| [PartIndex](../../aspose.cells.lowcode/splitpartinfo/partindex/) { get; } | Index of current part in sequence(0 based). -1 means there are no multiple parts so the result is single. |
| [SheetIndex](../../aspose.cells.lowcode/splitpartinfo/sheetindex/) { get; } | Index of the sheet where current part is in. -1 denotes there is only one sheet. |
| [SheetName](../../aspose.cells.lowcode/splitpartinfo/sheetname/) { get; } | Name of the sheet where current part is in. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassSplitPartInfoDemo
    {
        public static void Run()
        {
            try
            {
                // Create a workbook with multiple sheets for demonstration
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Worksheets.Add("Sheet2");
                workbook.Worksheets.Add("Sheet3");

                // Create LowCodeLoadOptions and LowCodeSplitOptions
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                loadOptions.InputFile = "sample.xlsx";

                LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
                splitOptions.LoadOptions = loadOptions;

                // Create a custom provider to demonstrate SplitPartInfo usage
                splitOptions.SaveOptionsProvider = new CustomSplitOptionsProvider();

                // Process the split operation
                SpreadsheetSplitter.Process(splitOptions);

                Console.WriteLine("Split operation completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomSplitOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Demonstrate accessing SplitPartInfo properties
            Console.WriteLine($"Processing part: Index={partInfo.PartIndex}, SheetIndex={partInfo.SheetIndex}, SheetName={partInfo.SheetName}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Part_{partInfo.PartIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


