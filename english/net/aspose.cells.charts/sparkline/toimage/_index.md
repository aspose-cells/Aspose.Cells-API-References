---
title: Sparkline.ToImage
second_title: Aspose.Cells for .NET API Reference
description: Sparkline method. Converts a sparkline to an image
type: docs
url: /net/aspose.cells.charts/sparkline/toimage/
---
## ToImage(ImageOrPrintOptions) {#toimage}

Converts a sparkline to an image.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | ImageOrPrintOptions | The image options |

### Return Value

Returns a Bitmap object.

### Examples

```csharp
namespace AsposeCellsExamples.SparklineMethodToImageWithImageOrPrintOptionsDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SparklineMethodToImageWithImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for sparkline
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(15);
            worksheet.Cells["A3"].PutValue(8);
            worksheet.Cells["A4"].PutValue(20);
            worksheet.Cells["A5"].PutValue(5);

            // Add a sparkline group
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Column, "A1:A5", false, new CellArea { StartRow = 0, StartColumn = 1, EndRow = 0, EndColumn = 1 });
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];
            Sparkline sparkline = group.Sparklines[0];

            // Create image options
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Jpeg,
                Quality = 100,
                HorizontalResolution = 200,
                VerticalResolution = 200
            };

            // Create output file path
            string outputPath = "SparklineOutput.jpg";

            try
            {
                // Call ToImage with file path and ImageOrPrintOptions
                sparkline.ToImage(outputPath, options);

                Console.WriteLine("Sparkline successfully converted to image and saved to: " + outputPath);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting sparkline to image: {ex.Message}");
            }

            // Save the workbook
            workbook.Save("SparklineToImageDemo.xlsx");
        }
    }
}
```

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_2}

Converts a sparkline to an image.

```csharp
public void ToImage(string fileName, ImageOrPrintOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The image file name. |
| options | ImageOrPrintOptions | The image options |

### Examples

```csharp
// Called: line.ToImage("output.png", options);
public static void Sparkline_Method_ToImage()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Define the CellArea for the sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Add a sparkline group to the worksheet
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Add a sparkline to the group
            idx = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);
            Sparkline line = group.Sparklines[idx];

            // Output sparkline details
            Console.WriteLine("Sparkline data range: " + line.DataRange + ", row: " + line.Row + ", column: " + line.Column);

            // Save the sparkline as an image
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            line.ToImage("output.png", options);

            // Save the workbook
            workbook.Save("SparklineExample.xlsx");
        }
```

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_1}

Converts a sparkline to an image.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The image stream. |
| options | ImageOrPrintOptions | The image options. |

### Examples

```csharp
namespace AsposeCellsExamples.SparklineMethodToImageWithStreamImageOrPrintOptionsDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SparklineMethodToImageWithStreamImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for sparkline
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(3);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["A4"].PutValue(2);
            worksheet.Cells["A5"].PutValue(9);

            // Add a sparkline group
            int groupIndex = worksheet.SparklineGroups.Add(Aspose.Cells.Charts.SparklineType.Line, "A1:A5", false, new CellArea { StartRow = 0, StartColumn = 1, EndRow = 0, EndColumn = 1 });
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];
            Sparkline sparkline = group.Sparklines[0];

            // Create image options
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300,
                Transparent = true
            };

            // Create memory stream for output
            using (MemoryStream stream = new MemoryStream())
            {
                try
                {
                    // Call ToImage with Stream and ImageOrPrintOptions
                    sparkline.ToImage(stream, options);

                    // Save the stream to a file
                    File.WriteAllBytes("SparklineImage.png", stream.ToArray());

                    Console.WriteLine("Sparkline successfully converted to image and saved.");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error converting sparkline to image: {ex.Message}");
                }
            }

            // Save the workbook
            workbook.Save("SparklineDemo.xlsx");
        }
    }
}
```

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


