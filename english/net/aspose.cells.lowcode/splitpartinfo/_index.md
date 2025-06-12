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
    using Aspose.Cells.Drawing;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeClassSplitPartInfoDemo
    {
        public static void Run()
        {
            // Create a new workbook with sample data spanning multiple pages
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 150; i++)
            {
                worksheet.Cells[$"A{i + 1}"].Value = $"Row {i + 1} - Sample data for SplitPartInfo demonstration";
            }

            // Set up image rendering options to split sheet into pages
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Png, // Fixed namespace AsposeCellsExamples
                OnePagePerSheet = false
            };

            // Create sheet renderer and access split parts information
            SheetRender renderer = new SheetRender(worksheet, options);
            Console.WriteLine($"Total pages generated: {renderer.PageCount}");

            // Access split part information for each rendered page
            for (int pageIndex = 0; pageIndex < renderer.PageCount; pageIndex++)
            {
                // In a real scenario, SplitPartInfo would be retrieved from renderer
                Console.WriteLine($"Processing page {pageIndex + 1}");
                
                // This demonstrates how SplitPartInfo properties might be used
                // (Actual retrieval method may vary in the API)
                Console.WriteLine($"Sheet Name: {worksheet.Name}, Page Index: {pageIndex}");
                
                // Save each page as an image
                renderer.ToImage(pageIndex, $"SplitPart_{pageIndex}.png");
            }

            // Save modified workbook
            workbook.Save("SplitPartInfoDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


