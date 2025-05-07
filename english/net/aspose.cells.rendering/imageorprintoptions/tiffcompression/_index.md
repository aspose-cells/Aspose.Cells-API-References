---
title: ImageOrPrintOptions.TiffCompression
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Gets or sets the type of compression to apply only when saving pages to the Tiff format
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/tiffcompression/
---
## ImageOrPrintOptions.TiffCompression property

Gets or sets the type of compression to apply only when saving pages to the `Tiff` format.

```csharp
public TiffCompression TiffCompression { get; set; }
```

### Remarks

Has effect only when saving to TIFF. The default value is Lzw.

### Examples

```csharp
// Called: imgOpt.TiffCompression = TiffCompression.CompressionCCITT4;
[Test]
        public void Property_TiffCompression()
        {
            Workbook wb = new Workbook(Constants.TemplatePath + "NetCoreTests/testToTiff.xlsx");

            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.HorizontalResolution = 300;
            imgOpt.VerticalResolution = 300;

            //PdfSaveOptions options = new PdfSaveOptions(SaveFormat.Pdf);
            //options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;

            imgOpt.ImageType = ImageType.Tiff;

            WorkbookRender wbRender;
            //please try the other tiff compressions.
            imgOpt.TiffCompression = TiffCompression.CompressionNone;
            //wbRender = new WorkbookRender(wb, imgOpt);
            //wbRender.ToImage(Constants.destPath + @"NetCoreTests\test_Cs_None.tiff");//too slow

            imgOpt.TiffCompression = TiffCompression.CompressionRle;
            //wbRender = new WorkbookRender(wb, imgOpt);
            //wbRender.ToImage(Constants.destPath + @"NetCoreTests\test_Cs_Rle.tiff");//too slow

            imgOpt.TiffCompression = TiffCompression.CompressionLZW;
            wbRender = new WorkbookRender(wb, imgOpt);
            wbRender.ToImage(Constants.destPath + @"NetCoreTests\test_Cs_LZW.tiff");

            imgOpt.TiffCompression = TiffCompression.CompressionCCITT3;
            wbRender = new WorkbookRender(wb, imgOpt);
            wbRender.ToImage(Constants.destPath + @"NetCoreTests\test_Cs_CCITT3.tiff");

            imgOpt.TiffCompression = TiffCompression.CompressionCCITT4;
            wbRender = new WorkbookRender(wb, imgOpt);
            wbRender.ToImage(Constants.destPath + @"NetCoreTests\test_Cs_CCITT4.tiff");


        }
```

### See Also

* enum [TiffCompression](../../tiffcompression/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


