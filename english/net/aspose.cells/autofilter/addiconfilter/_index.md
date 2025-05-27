---
title: AutoFilter.AddIconFilter
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Adds an icon filter
type: docs
url: /net/aspose.cells/autofilter/addiconfilter/
---
## AutoFilter.AddIconFilter method

Adds an icon filter.

```csharp
public void AddIconFilter(int fieldIndex, IconSetType iconSetType, int iconId)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| iconSetType | IconSetType | The icon set type. |
| iconId | Int32 | The icon id. |

### Remarks

Only supports to add the icon filter. Not supports checking which row is visible if the filter is icon filter.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodAddIconFilterWithInt32IconSetTypeInt32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Populate sample data in column A
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(50);

            // Get auto filter instance
            AutoFilter autoFilter = worksheet.AutoFilter;
            
            // Set autofilter range (A1:A6) using startRow, startColumn, endRow
            autoFilter.SetRange(0, 0, 5);

            try
            {
                // Add icon filter to first column (fieldIndex: 0)
                // Using 3 Traffic Lights icon set (IconSetType.TrafficLights31)
                // Filtering for first icon in set (iconId: 0)
                autoFilter.AddIconFilter(0, IconSetType.TrafficLights31, 0);
                
                // Refresh filter to apply changes
                autoFilter.Refresh();

                Console.WriteLine("Added icon filter to column A showing items with first traffic light icon");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddIconFilter: {ex.Message}");
            }

            // Save the modified workbook
            workbook.Save("AddIconFilterDemo.xlsx");
        }
    }
}
```

### See Also

* enum [IconSetType](../../iconsettype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


