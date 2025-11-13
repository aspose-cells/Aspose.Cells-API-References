---
title: Class ColorFilter
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ColorFilter class. Represents setting for filtering the range by color
type: docs
url: /net/aspose.cells/colorfilter/
---
## ColorFilter class

Represents setting for filtering the range by color.

```csharp
public class ColorFilter
```

## Properties

| Name | Description |
| --- | --- |
| [FilterByFillColor](../../aspose.cells/colorfilter/filterbyfillcolor/) { get; set; } | Whether filter by the cell's fill color. |

## Methods

| Name | Description |
| --- | --- |
| [GetColor](../../aspose.cells/colorfilter/getcolor/)(WorksheetCollection) | Gets the color of this filter. |

### Examples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassColorFilterDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data with different colors
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Red");
            cells["A2"].PutValue("Green");
            cells["A3"].PutValue("Blue");
            cells["A4"].PutValue("Red");
            
            // Apply colors to cells
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = Color.Red;
            style1.Pattern = BackgroundType.Solid;
            cells["A1"].SetStyle(style1);
            cells["A4"].SetStyle(style1);
            
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = Color.Green;
            style2.Pattern = BackgroundType.Solid;
            cells["A2"].SetStyle(style2);
            
            Style style3 = workbook.CreateStyle();
            style3.ForegroundColor = Color.Blue;
            style3.Pattern = BackgroundType.Solid;
            cells["A3"].SetStyle(style3);
            
            // Create auto filter
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Create color filter for red cells
            CellsColor cr = workbook.CreateCellsColor();
            cr.Color = Color.Red;
            filter.AddFillColorFilter(0, BackgroundType.Solid, cr, cr);
            filter.Refresh();
            
            // Check filtered rows
            Console.WriteLine("Row 1 hidden: " + cells.IsRowHidden(0));
            Console.WriteLine("Row 2 hidden: " + cells.IsRowHidden(1));
            Console.WriteLine("Row 3 hidden: " + cells.IsRowHidden(2));
            Console.WriteLine("Row 4 hidden: " + cells.IsRowHidden(3));
            
            // Access the color filter
            FilterColumn fc = filter.FilterColumns[0];
            ColorFilter cf = fc.Filter as ColorFilter;
            
            Console.WriteLine("Filter by fill color: " + cf.FilterByFillColor);
            Console.WriteLine("Filter color: " + cf.GetColor(workbook.Worksheets));
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


