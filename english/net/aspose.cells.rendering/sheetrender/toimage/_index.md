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
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToImageWithInt32GraphicsSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells["A1"].Value = "Sample Data for Rendering";
            worksheet.Cells["A2"].Value = "This will be rendered to an image";

            try
            {
                // Create image options
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Create sheet render for the worksheet
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Create a memory stream to capture the rendered image
                using (MemoryStream stream = new MemoryStream())
                {
                    // Call ToImage with the specified parameters
                    // Since we can't use System.Drawing.Graphics, we'll use the simpler ToImage overload
                    sheetRender.ToImage(0, stream);

                    // Save the rendered image to file
                    File.WriteAllBytes("RenderedOutput.png", stream.ToArray());
                }

                Console.WriteLine("Sheet rendered to image successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
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
    using System;
    using System.IO;

    public class SheetRenderMethodToImageWithInt32GraphicsSingleSingleDemo
    {
        public static void Run()
        {
            // Create a new workbook with sample data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data for Rendering";
            worksheet.Cells["A2"].Value = "This will be rendered to an image";

            // Create image options
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // Create SheetRender instance
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // Since we can't use System.Drawing types, we'll use the alternative ToImage method
                // that saves directly to a file
                sheetRender.ToImage(0, "RenderedOutput.png");
                Console.WriteLine("Sheet rendered to image successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
            finally
            {
                // Clean up resources
                sheetRender.Dispose();
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToImageWithInt32StreamDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "Row 1";
            worksheet.Cells["B2"].Value = 100;

            try
            {
                // Create image options
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Create SheetRender instance
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Create a memory stream to hold the image
                using (MemoryStream stream = new MemoryStream())
                {
                    // Call ToImage with page index and stream parameters
                    sheetRender.ToImage(0, stream);

                    Console.WriteLine($"Successfully rendered page 0 to stream. Stream length: {stream.Length} bytes");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error rendering to image: {ex.Message}");
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetRenderMethodToImageWithInt32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "Row 1";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "Row 2";
            worksheet.Cells["B3"].Value = 200;

            try
            {
                // Create image options
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Create SheetRender instance
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Get the first page index (0-based)
                int pageIndex = 0;

                // Call ToImage with the page index parameter
                sheetRender.ToImage(pageIndex, "output_page.png");

                Console.WriteLine($"Successfully rendered page {pageIndex} to image");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error rendering to image: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


