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
| [IconSetType](../../aspose.cells/iconfilter/iconsettype/) { get; set; } | Gets and sets which icon set is used in the filter criteria. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    
    public class CellsClassIconFilterDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }
            
            // Create auto filter
            worksheet.AutoFilter.Range = "A1:A10";
            
            // Apply the icon filter directly using AddIconFilter
            worksheet.AutoFilter.AddIconFilter(0, IconSetType.Arrows3, 1);
            
            // Save the result
            workbook.Save("IconFilterDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


