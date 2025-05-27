---
title: DrawObject.CurrentPage
second_title: Aspose.Cells for .NET API Reference
description: DrawObject property. Indicates the page index of DrawObject. Page index is based on zero. One Sheet contains several pages when rendering
type: docs
url: /net/aspose.cells.rendering/drawobject/currentpage/
---
## DrawObject.CurrentPage property

Indicates the page index of DrawObject. Page index is based on zero. One Sheet contains several pages when rendering.

```csharp
public int CurrentPage { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class DrawObjectPropertyCurrentPageDemo
    {
        public static void Run()
        {
            // Create a workbook and add some data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            // Add a second worksheet to demonstrate multi-page rendering
            workbook.Worksheets.Add();
            worksheet = workbook.Worksheets[1];
            worksheet.Cells["B2"].PutValue("Second Page Data");

            // Set up image or print options
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = false;

            // Create a sheet render for the first worksheet
            SheetRender render = new SheetRender(workbook.Worksheets[0], options);

            // Demonstrate CurrentPage property during rendering
            for (int pageIndex = 0; pageIndex < render.PageCount; pageIndex++)
            {
                // Create a DrawObject by implementing IDrawObject interface
                var drawObject = new CustomDrawObject
                {
                    CurrentPage = pageIndex + 1,
                    TotalPages = render.PageCount,
                    SheetIndex = 0
                };

                Console.WriteLine($"Sheet Index: {drawObject.SheetIndex}, Current Page: {drawObject.CurrentPage}, Total Pages: {drawObject.TotalPages}");
            }
        }
    }

    // Custom implementation of DrawObject properties
    public class CustomDrawObject : IDrawObject
    {
        public int CurrentPage { get; set; }
        public int TotalPages { get; set; }
        public int SheetIndex { get; set; }
    }

    // Minimal interface definition
    public interface IDrawObject
    {
        int CurrentPage { get; set; }
        int TotalPages { get; set; }
        int SheetIndex { get; set; }
    }
}
```

### See Also

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


