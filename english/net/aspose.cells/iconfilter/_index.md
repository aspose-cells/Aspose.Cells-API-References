---
title: Class IconFilter
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.IconFilter class. Represents icon filter
type: docs
url: /net/aspose.cells/iconfilter/
---
## IconFilter class

Represents icon filter.

```csharp
public class IconFilter
```

## Properties

| Name | Description |
| --- | --- |
| [IconId](../../aspose.cells/iconfilter/iconid/) { get; set; } | Gets and sets Zero-based index of an icon in an icon set. |
| [IconSetType](../../aspose.cells/iconfilter/iconsettype/) { get; set; } | Gets and sets which icon set is used for this filter criteria. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassIconFilterDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Populate sample data
                for (int i = 0; i < 10; i++)
                {
                    worksheet.Cells[i, 0].PutValue(i * 10);
                }

                // Create auto filter
                worksheet.AutoFilter.Range = "A1:A10";
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
                filterColumn.FilterType = FilterType.IconFilter;

                // Get the icon filter
                IconFilter iconFilter = (IconFilter)filterColumn.Filter;

                // Set icon filter properties
                iconFilter.IconSetType = IconSetType.Arrows3;
                iconFilter.IconId = 1; // Filter for middle arrow

                Console.WriteLine($"IconFilter created with IconSetType: {iconFilter.IconSetType} and IconId: {iconFilter.IconId}");

                // Save the workbook
                workbook.Save("IconFilterDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with icon filter applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with IconFilter: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


