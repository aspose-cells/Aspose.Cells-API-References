---
title: SplitPartInfo.SheetIndex
second_title: Aspose.Cells for .NET API Reference
description: SplitPartInfo property. Index of the sheet where current part is in. 1 denotes there is only one sheet
type: docs
url: /net/aspose.cells.lowcode/splitpartinfo/sheetindex/
---
## SplitPartInfo.SheetIndex property

Index of the sheet where current part is in. -1 denotes there is only one sheet.

```csharp
public int SheetIndex { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SplitPartInfoPropertySheetIndexDemo
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
                splitOptions.SaveOptionsProvider = new CustomSheetIndexProvider();

                // Process the split operation
                SpreadsheetSplitter.Process(splitOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomSheetIndexProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Demonstrate reading the SheetIndex property
            Console.WriteLine($"Current part SheetIndex: {partInfo.SheetIndex}");
            Console.WriteLine($"Current part SheetName: {partInfo.SheetName}");
            Console.WriteLine($"Current part PartIndex: {partInfo.PartIndex}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Sheet_{partInfo.SheetIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### See Also

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


