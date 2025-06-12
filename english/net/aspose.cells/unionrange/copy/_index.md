---
title: UnionRange.Copy
second_title: Aspose.Cells for .NET API Reference
description: UnionRange method. Copying the range with paste special options
type: docs
url: /net/aspose.cells/unionrange/copy/
---
## UnionRange.Copy method

Copying the range with paste special options.

```csharp
public void Copy(UnionRange range, PasteOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| range | UnionRange | The source range. |
| options | PasteOptions | The paste special options. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodCopyWithUnionRangePasteOptionsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fill some data in the source range
            worksheet.Cells["A1"].PutValue("Source Data 1");
            worksheet.Cells["A2"].PutValue("Source Data 2");
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);

            // Create source UnionRange
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:B2");

            // Create destination UnionRange
            Aspose.Cells.Range destRange = worksheet.Cells.CreateRange("D1:E2");

            // Create PasteOptions to skip blanks and transpose
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.SkipBlanks = true;
            pasteOptions.Transpose = true;

            try
            {
                // Call the Copy method with UnionRange and PasteOptions
                sourceRange.Copy(destRange, pasteOptions);

                Console.WriteLine("Copy method executed successfully with parameters (UnionRange, PasteOptions)");
                Console.WriteLine("Source range A1:B2 has been copied to D1:E2 with transposition");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Copy method: {ex.Message}");
            }

            // Save the result
            workbook.Save("UnionRangeCopyDemo.xlsx");
        }
    }
}
```

### See Also

* class [PasteOptions](../../pasteoptions/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


