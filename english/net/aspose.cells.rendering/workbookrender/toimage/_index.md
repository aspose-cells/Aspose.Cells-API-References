---
title: WorkbookRender.ToImage
second_title: Aspose.Cells for .NET API Reference
description: WorkbookRender method. Render whole workbook as Tiff Image to stream
type: docs
url: /net/aspose.cells.rendering/workbookrender/toimage/
---
## ToImage(Stream) {#toimage_3}

Render whole workbook as Tiff Image to stream.

```csharp
public void ToImage(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | the stream of the output image |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class WorkbookRenderMethodToImageWithStreamDemo
    {
        public static void Run()
        {
            // Create a new workbook with sample data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Aspose.Cells ToImage Stream Demo";

            // Configure image rendering options
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png; // Fixed namespace AsposeCellsExamples

            // Create output directory if it doesn't exist
            string outputDir = "output/";
            Directory.CreateDirectory(outputDir);

            // Create a file stream for image output
            string imagePath = Path.Combine(outputDir, "workbook_render.png");
            using (FileStream imageStream = new FileStream(imagePath, FileMode.Create))
            {
                try
                {
                    // Initialize workbook renderer and convert to image
                    WorkbookRender renderer = new WorkbookRender(workbook, options); // Removed using statement
                    renderer.ToImage(imageStream);

                    Console.WriteLine($"Workbook rendered successfully to: {imagePath}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error during rendering: {ex.Message}");
                }
            }

            // Save the original workbook for reference
            workbook.Save(Path.Combine(outputDir, "source_workbook.xlsx"));
        }
    }
}
```

### See Also

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_4}

Render whole workbook as Tiff Image to a file.

```csharp
public void ToImage(string filename)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filename | String | the filename of the output image |

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodToImageWithStringDemo
    {
        public static void Run()
        {
            // Create a sample workbook
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("Test ToImage Method");
            
            // Set image options
            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.ImageType = ImageType.Tiff;
            imgOpt.TiffCompression = TiffCompression.CompressionLZW;
            imgOpt.HorizontalResolution = 300;
            imgOpt.VerticalResolution = 300;

            // Create workbook render and save to image
            WorkbookRender wbRender = new WorkbookRender(wb, imgOpt);
            string outputPath = "output.tiff";
            wbRender.ToImage(outputPath);
            
            Console.WriteLine("Workbook rendered to image: " + outputPath);
        }
    }
}
```

### See Also

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, string) {#toimage_2}

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
    public class WorkbookRenderMethodToImageWithInt32StringDemo
    {
        public static void Run()
        {
            // Create a new workbook with sample data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Create image options
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true
            };

            // Create workbook renderer
            WorkbookRender renderer = new WorkbookRender(workbook, options);

            // Save each page as image
            for (int i = 0; i < renderer.PageCount; i++)
            {
                renderer.ToImage(i, $"output_page_{i}.png");
            }
        }
    }
}
```

### See Also

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Stream) {#toimage_1}

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
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class WorkbookRenderMethodToImageWithInt32StreamDemo
    {
        public static void Run()
        {
            // Create a new workbook with sample data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data for Rendering");

            // Configure image rendering options
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Png, // Namespace reference fixed via using directive
                OnePagePerSheet = true
            };

            // Create workbook render (removed using statement since it doesn't implement IDisposable)
            WorkbookRender render = new WorkbookRender(workbook, options);
            {
                if (render.PageCount < 1)
                {
                    Console.WriteLine("No pages available for rendering");
                    return;
                }

                try
                {
                    // Create output stream for image
                    using (FileStream imageStream = new FileStream("output_page.png", FileMode.Create))
                    {
                        // Render first page to stream
                        render.ToImage(0, imageStream);
                    }

                    Console.WriteLine("Successfully converted first page to PNG image");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error during image conversion: {ex.Message}");
                }
            }

            // Save original workbook for reference
            workbook.Save("RenderingDemoWorkbook.xlsx");
        }
    }
}
```

### See Also

* class [WorkbookRender](../)
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
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class WorkbookRenderMethodToImageWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample content to demonstrate rendering
            worksheet.Cells["A1"].PutValue("Aspose.Cells ToImage Demo");
            worksheet.Cells["B3"].PutValue(DateTime.Now.ToString());
            worksheet.AutoFitColumn(0);

            // Configure image rendering options
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Png,
                OnePagePerSheet = true
            };

            WorkbookRender renderer = new WorkbookRender(workbook, options);
            try
            {
                if (renderer.PageCount == 0)
                {
                    Console.WriteLine("No pages available for rendering.");
                    return;
                }

                // Render first page to PNG image
                renderer.ToImage(0, "output_page_0.png");
                Console.WriteLine($"Successfully rendered page 1 of {renderer.PageCount} to output_page_0.png");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }

            // Save original workbook for reference
            workbook.Save("WorkbookRenderToImageDemo.xlsx");
        }
    }
}
```

### See Also

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


