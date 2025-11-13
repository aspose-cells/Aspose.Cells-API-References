---
title: FilterColumn.Filter
second_title: Aspose.Cells for .NET API Reference
description: FilterColumn property. Gets and sets the condition of filtering data
type: docs
url: /net/aspose.cells/filtercolumn/filter/
---
## FilterColumn.Filter property

Gets and sets the condition of filtering data.

```csharp
[Obsolete("Use FilterColumn.MultipleFilters,CustomFilters and so on... property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public object Filter { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead,please use FilterColumn.MultipleFilters,CustomFilters and so on... property according to differnt type of filter /// This property will be removed 12 months later since October 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFilterDemo
    {
        public static void Run()
        {
            // Create a workbook with sample data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data with color formatting
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Color");
            cells["A2"].PutValue("Red");
            cells["A3"].PutValue("Red");
            cells["A4"].PutValue("Blue");
            
            // Format cells with colors
            Style redStyle = workbook.CreateStyle();
            redStyle.ForegroundColor = Color.Red;
            redStyle.Pattern = BackgroundType.Solid;
            
            Style blueStyle = workbook.CreateStyle();
            blueStyle.ForegroundColor = Color.Blue;
            blueStyle.Pattern = BackgroundType.Solid;
            
            cells["A2"].SetStyle(redStyle);
            cells["A3"].SetStyle(redStyle);
            cells["A4"].SetStyle(blueStyle);
            
            // Apply auto filter
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Add color filter for red cells
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            filter.Refresh();
            
            // Access the filter column and its Filter property
            FilterColumn fc = filter.FilterColumns[0];
            ColorFilter cf = fc.Filter as ColorFilter;
            
            // Output filter properties
            Console.WriteLine($"Filter type: {fc.FilterType}");
            Console.WriteLine($"Filter by fill color: {cf.FilterByFillColor}");
            Console.WriteLine($"Filter color: {cf.GetColor(workbook.Worksheets)}");
            
            // Save the workbook
            workbook.Save("ColorFilterDemo.xlsx");
        }
    }
}
```

### See Also

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


