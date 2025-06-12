---
title: PicFormatOption.Type
second_title: Aspose.Cells for .NET API Reference
description: PicFormatOption property. Gets or sets the picture fill type
type: docs
url: /net/aspose.cells.drawing/picformatoption/type/
---
## PicFormatOption.Type property

Gets or sets the picture fill type.

```csharp
public FillPictureType Type { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a rectangle shape
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 200);

            // Configure picture fill
            FillFormat fill = shape.Fill;
            fill.FillType = FillType.Texture;
            fill.ImageData = GenerateSampleImage();

            // Access picture format options via FillFormat properties
            Console.WriteLine("Initial Fill Type: " + fill.PictureFormatType);
            fill.PictureFormatType = FillPictureType.Stack;
            fill.Scale = 0.25; // Shows 4 stacked tiles at 25% scale

            // Save modified workbook
            workbook.Save("PicFormatTypeDemo.xlsx");
        }

        private static byte[] GenerateSampleImage()
        {
            // Generate 2x2 pixel BMP with red/blue pattern
            using (MemoryStream ms = new MemoryStream())
            using (BinaryWriter writer = new BinaryWriter(ms))
            {
                // BMP header (54 bytes)
                writer.Write(new char[] { 'B', 'M' });
                writer.Write(54 + 12); // File size
                writer.Write(0); // Reserved
                writer.Write(54); // Data offset
                writer.Write(40); // Header size
                writer.Write(2); // Width
                writer.Write(2); // Height
                writer.Write((short)1); // Planes
                writer.Write((short)24); // BPP
                writer.Write(0); // Compression
                writer.Write(0); // Image size
                writer.Write(0); // XPPM
                writer.Write(0); // YPPM
                writer.Write(0); // Colors
                writer.Write(0); // Important colors

                // Pixel data (2x2 pattern)
                writer.Write(new byte[] { 255, 0, 0 }); // Blue pixel
                writer.Write(new byte[] { 0, 0, 255 }); // Red pixel
                writer.Write(new byte[] { 0, 0, 255 }); // Red pixel
                writer.Write(new byte[] { 255, 0, 0 }); // Blue pixel
                writer.Write(0); // Row padding

                return ms.ToArray();
            }
        }
    }
}
```

### See Also

* enum [FillPictureType](../../fillpicturetype/)
* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


