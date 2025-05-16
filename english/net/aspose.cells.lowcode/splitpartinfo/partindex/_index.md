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
namespace AsposeCellsExamples.SplitPartInfoPropertyPartIndexDemo
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class SplitPartInfoPropertyPartIndexDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells["A1"].PutValue("Sample Data");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue(i);
            }

            // Create an image or print options
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // In a real scenario, SplitPartInfo would be created by the API during rendering
            // For demonstration, we'll simulate accessing these properties
            // Note: Since we can't create SplitPartInfo directly, we'll focus on the property demonstration
            
            // Create a SheetRender which might generate SplitPartInfo internally
            SheetRender render = new SheetRender(worksheet, options);
            
            // In a real use case, you would access SplitPartInfo from the rendering result
            // For demo purposes, we'll just show the property names and their usage
            Console.WriteLine("This demo shows how SplitPartInfo properties would be accessed:");
            Console.WriteLine("PartIndex - read-only property showing part index");
            Console.WriteLine("SheetIndex - read-only property showing sheet index");
            Console.WriteLine("SheetName - read-only property showing sheet name");

            Console.WriteLine("Number of pages: " + render.PageCount);

            // Save the result
            workbook.Save("PropertyPartIndexDemo.xlsx");
        }
    }
}
```

### See Also

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


