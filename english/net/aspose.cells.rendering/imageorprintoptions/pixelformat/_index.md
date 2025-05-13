---
title: ImageOrPrintOptions.PixelFormat
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Gets or sets the pixel format for the generated images
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/pixelformat/
---
## ImageOrPrintOptions.PixelFormat property

Gets or sets the pixel format for the generated images.

```csharp
public PixelFormat PixelFormat { get; set; }
```

### Remarks

The default value is PixelFormat.Format32bppArgb.

### Examples

```csharp
// Called: cellRenderoptions.PixelFormat = System.Drawing.Imaging.PixelFormat.Format32bppArgb;
public void ImageOrPrintOptions_Property_PixelFormat()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");

    var selectedWS = wb.Worksheets[0];

    Aspose.Cells.PageSetup setup = selectedWS.PageSetup;
    setup.PaperSize = Aspose.Cells.PaperSizeType.PaperA4;
    int horizDpi = 170;
    int vertDpi = 170;
    Aspose.Cells.Rendering.ImageOrPrintOptions cellRenderoptions = new Aspose.Cells.Rendering.ImageOrPrintOptions();

    // Set Horizontal Resolution
    cellRenderoptions.ImageType = ImageType.Tiff;
    cellRenderoptions.TiffCompression = Aspose.Cells.Rendering.TiffCompression.CompressionCCITT3;

    // Set Vertical Resolution
    cellRenderoptions.VerticalResolution = vertDpi;
    cellRenderoptions.HorizontalResolution = horizDpi;
    cellRenderoptions.Quality = 100;
    cellRenderoptions.SmoothingMode = System.Drawing.Drawing2D.SmoothingMode.HighQuality;
    cellRenderoptions.PixelFormat = System.Drawing.Imaging.PixelFormat.Format32bppArgb;

    // If you want entire sheet as a single image
    cellRenderoptions.OnePagePerSheet = false;


    // Render to image
    Aspose.Cells.Rendering.SheetRender sr = new Aspose.Cells.Rendering.SheetRender(selectedWS, cellRenderoptions);
    MemoryStream ms = new MemoryStream();
    sr.ToTiff(ms);

    int blackPointCount = 0;
    using (Bitmap b = (Bitmap)Image.FromStream(ms))
    {
        for (int i = 1002; i <= 1078; i++)
        {
            for (int j = 1593; j <= 1667; j++)
            {
                Color c = b.GetPixel(i, j);
                if (c.R == 0 && c.G == 0 && c.B == 0)
                {
                    blackPointCount++;
                }
            }
        }
    }
    Assert.IsTrue(blackPointCount > 1000);
}
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


