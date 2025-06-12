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
            // Create a new workbook with multiple sheets
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Simulate processing that generates SplitPartInfo instances (hypothetical scenario)
            // Assume GetSplitParts is a method that returns SplitPartInfo collection during conversion
            SplitPartInfo[] parts = GetSplitPartsSimulated(workbook);

            // Iterate through each SplitPartInfo and display SheetIndex
            foreach (SplitPartInfo part in parts)
            {
                Console.WriteLine($"Part Index: {part.PartIndex}, Sheet Index: {part.SheetIndex}, Sheet Name: {part.SheetName}");
            }
        }

        // Simulate method to obtain SplitPartInfo instances (illustrative purposes only)
        private static SplitPartInfo[] GetSplitPartsSimulated(Workbook workbook)
        {
            // In real usage, this would be populated by a method like ConvertWorkbookToParts()
            return new SplitPartInfo[]
            {
                new SplitPartInfo { /* Simulated data */ PartIndex = 0, SheetIndex = 0, SheetName = "Sheet1" },
                new SplitPartInfo { /* Simulated data */ PartIndex = 1, SheetIndex = 1, SheetName = "Sheet2" }
            };
        }
    }

    // Helper class to simulate SplitPartInfo instantiation (not part of actual Aspose.Cells API)
    internal class SplitPartInfo
    {
        public int PartIndex { get; set; }
        public int SheetIndex { get; set; }
        public string SheetName { get; set; }
    }
}
```

### See Also

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


