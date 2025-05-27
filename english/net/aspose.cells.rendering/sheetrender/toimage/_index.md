---
title: SheetRender.ToImage
second_title: Aspose.Cells for .NET API Reference
description: SheetRender method. Render certain page to a Graphics
type: docs
url: /net/aspose.cells.rendering/sheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

Render certain page to a Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indicate which page is to be converted |
| g | Graphics | The object where to render to. |
| x | Single | The X coordinate (in pixels) of the top left corner of the rendered page. |
| y | Single | The Y coordinate (in pixels) of the top left corner of the rendered page. |
| width | Single | The maximum width (in pixels) that can be occupied by the rendered page. |
| height | Single | The maximum height (in pixels) that can be occupied by the rendered page. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetRenderMethodToImageWithInt32GraphicsSingleSingleSinglDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells ToImage Demo");

            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Png,
                OnePagePerSheet = true
            };

            SheetRender sheetRender = new SheetRender(worksheet, options);
            {
                try
                {
                    // Use the ToImage overload that directly saves to file
                    sheetRender.ToImage(0, "SheetToGraphics.png");
                    Console.WriteLine("Worksheet rendered successfully to image");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error rendering worksheet: {ex.Message}");
                }
            }

            workbook.Save("ToImageDemoWorkbook.xlsx");
        }
    }
}
```

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

Render certain page to a Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indicate which page is to be converted |
| g | Graphics | The object where to render to. |
| x | Single | The X coordinate (in pixels) of the top left corner of the rendered page. |
| y | Single | The Y coordinate (in pixels) of the top left corner of the rendered page. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System;

    public class SheetRenderMethodToImageWithInt32GraphicsSingleSingleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Rendered to Image";

            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Png,
                OnePagePerSheet = true
            };

            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                sheetRender.ToImage(0, "SheetToImage.png");
                Console.WriteLine("Image created successfully with ToImage(Int32, Graphics, Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ToImageDemoWorkbook.xlsx");
        }
    }
}
```

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, string) {#toimage_4}

Render certain page to a file.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indicate which page is to be converted |
| fileName | String | filename of the output image |

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodToImageWithInt32StringDemo
    {
        public static void Run()
        {
            // Load the source Excel file
            Workbook workbook = new Workbook("Book1.xlsx");
            
            // Create image options
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Create sheet render for the first worksheet
            SheetRender sheetRender = new SheetRender(workbook.Worksheets[0], options);
            
            // Render the first page of the sheet to an image file
            sheetRender.ToImage(0, "output.png");
            
            Console.WriteLine("Sheet rendered to image successfully.");
        }
    }
}
```

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Stream) {#toimage_3}

Render certain page to a stream.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indicate which page is to be converted |
| stream | Stream | the stream of the output image |

### Examples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodToImageWithInt32StreamDemo
    {
        public static void Run()
        {
            // Create a workbook from sample Excel file
            Workbook workbook = new Workbook("example.xlsx");
            
            // Set image options
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Get the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Create sheet renderer
            SheetRender renderer = new SheetRender(worksheet, options);
            
            // Create output directory if it doesn't exist
            string outputDir = "output/";
            if (!Directory.Exists(outputDir))
            {
                Directory.CreateDirectory(outputDir);
            }
            
            // Render first page to stream
            using (Stream stream = File.Create(outputDir + "output.png"))
            {
                renderer.ToImage(0, stream);
            }
        }
    }
}
```

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int) {#toimage}

Render certain page to a Bitmap object.

```csharp
public Bitmap ToImage(int pageIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indicate which page is to be converted |

### Return Value

the bitmap object of the page

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodToImageWithInt32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access first worksheet and set some sample data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text");
            
            // Set image options
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                OnePagePerSheet = true
            };
            
            // Create sheet render
            SheetRender render = new SheetRender(worksheet, options);
            
            // Convert first page to image (page index 0)
            render.ToImage(0, "output.png");
        }
    }
}
```

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


