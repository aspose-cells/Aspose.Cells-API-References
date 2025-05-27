---
title: Shape.ToImage
second_title: Aspose.Cells for .NET API Reference
description: Shape method. Creates the shape image and saves it to a stream in the specified format
type: docs
url: /net/aspose.cells.drawing/shape/toimage/
---
## ToImage(Stream, ImageType) {#toimage_1}

Creates the shape image and saves it to a stream in the specified format.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The output stream. |
| imageType | ImageType | The type in which to save the image. |

### Remarks

The following formats are supported: .bmp, .gif, .jpg, .jpeg, .tiff, .emf.

### Examples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodToImageWithStreamImageTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a sample shape with correct parameters
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Convert shape to image stream
            using (MemoryStream imageStream = new MemoryStream())
            {
                shape.ToImage(imageStream, ImageType.Png);
                Console.WriteLine("Shape converted to image stream successfully");
            }
        }
    }
}
```

### See Also

* enum [ImageType](../../imagetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_3}

Saves the shape to a file.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ShapeMethodToImageWithStringImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a sample shape with all required parameters
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Set image options
            ImageOrPrintOptions options = new ImageOrPrintOptions()
            {
                HorizontalResolution = 300,
                VerticalResolution = 300
            };

            // Save shape to image
            shape.ToImage("shape_image.png", options);
        }
    }
}
```

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_2}

Saves the shape to a stream.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

### Examples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ShapeMethodToImageWithStreamImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a sample shape
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Create memory stream for output
            MemoryStream imageStream = new MemoryStream();

            // Set image options
            ImageOrPrintOptions options = new ImageOrPrintOptions()
            {
                ImageType = ImageType.Png,
                OnePagePerSheet = true
            };

            // Convert shape to image
            shape.ToImage(imageStream, options);

            // Reset stream position for demonstration (actual usage would save/process the stream)
            imageStream.Position = 0;
        }
    }
}
```

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage}

Returns the bitmap object of the shape .

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

### Examples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ShapeMethodToImageWithImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a sample shape to the worksheet
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Set ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;

            // Convert shape to image with options
            MemoryStream imageStream = new MemoryStream();
            shape.ToImage(imageStream, options);

            // Save the image to file
            using (FileStream file = new FileStream("ShapeImage.png", FileMode.Create))
            {
                imageStream.WriteTo(file);
            }
        }
    }
}
```

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


