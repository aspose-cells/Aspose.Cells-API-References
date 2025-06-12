---
title: DrawObject.TotalPages
second_title: Aspose.Cells for .NET API Reference
description: DrawObject property. Indicates total pages in current rendering
type: docs
url: /net/aspose.cells.rendering/drawobject/totalpages/
---
## DrawObject.TotalPages property

Indicates total pages in current rendering.

```csharp
public int TotalPages { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class DrawObjectPropertyTotalPagesDemo
    {
        public static void Run()
        {
            // Create a workbook and add some data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data
            worksheet.Cells["A1"].PutValue("Sample Data");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue($"Item {i-1}");
            }

            // Add a second worksheet
            workbook.Worksheets.Add();
            
            // Create image or print options
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = false;

            // Create sheet render
            SheetRender render = new SheetRender(worksheet, options);

            // Demonstrate TotalPages property
            Console.WriteLine($"Total pages to render: {render.PageCount}");

            // Simulate drawing each page
            for (int pageIndex = 0; pageIndex < render.PageCount; pageIndex++)
            {
                Console.WriteLine($"Rendering page {pageIndex + 1} of {render.PageCount}");
                
                // In a real scenario, you would render the page here
                // render.ToImage(pageIndex, "output_" + pageIndex + ".png");
            }
        }
    }
}
```

### See Also

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


