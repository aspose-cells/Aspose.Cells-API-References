---
title: Enum PasteType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.PasteType enum. Represents the paste special type
type: docs
url: /net/aspose.cells/pastetype/
---
## PasteType enumeration

Represents the paste special type.

```csharp
public enum PasteType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| All | `0` | Copies all data of the range. |
| Default | `1` | It works as "All" behavior of MS Excel. |
| AllExceptBorders | `2` | Copies all data of the range without the range. |
| DefaultExceptBorders | `3` | It works as "All except borders" behavior of MS Excel. |
| ColumnWidths | `4` | Only copies the widths of the range. |
| RowHeights | `5` | Only copies the heights of the range. |
| Comments | `6` |  |
| Formats | `7` |  |
| Formulas | `8` |  |
| FormulasAndNumberFormats | `9` |  |
| Validation | `10` |  |
| Values | `11` |  |
| ValuesAndFormats | `12` |  |
| ValuesAndNumberFormats | `13` |  |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PasteTypeDemo
    {
        public static void PasteTypeExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Define the source range
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:B4");

            // Define the destination range
            Aspose.Cells.Range destinationRange = worksheet.Cells.CreateRange("D1:E4");

            // Create PasteOptions and set the PasteType
            PasteOptions pasteOptions = new PasteOptions
            {
                PasteType = PasteType.Values,
                SkipBlanks = true,
                OnlyVisibleCells = false,
                Transpose = false,
                IgnoreLinksToOriginalFile = true
            };

            // Copy the source range to the destination range with the specified paste options
            destinationRange.Copy(sourceRange, pasteOptions);

            // Save the workbook
            workbook.Save("PasteTypeExample.xlsx");

            // Output the results
            Console.WriteLine("Data copied with PasteType.Values and saved to PasteTypeExample.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


