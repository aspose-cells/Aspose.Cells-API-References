---
title: Enum TiffCompression
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Rendering.TiffCompression enum. Specifies what type of compression to apply when saving images into TIFF format file
type: docs
url: /net/aspose.cells.rendering/tiffcompression/
---
## TiffCompression enumeration

Specifies what type of compression to apply when saving images into TIFF format file.

```csharp
public enum TiffCompression
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| CompressionNone | `0` | Specifies no compression. |
| CompressionRle | `1` | Specifies the RLE compression scheme. |
| CompressionLZW | `2` | Specifies the LZW compression scheme. |
| CompressionCCITT3 | `3` | Specifies the CCITT3 compression scheme. |
| CompressionCCITT4 | `4` | Specifies the CCITT4 compression scheme. |

### Examples

```csharp
// Called: imgOpt.TiffCompression = TiffCompression.CompressionLZW;
[Test]
        public void Type_TiffCompression()
        {
            Workbook wb = new Workbook(Constants.TemplatePath + &quot;NetCoreTests/testToTiff.xlsx&quot;);

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
            //wbRender.ToImage(Constants.destPath + @&quot;NetCoreTests\test_Cs_None.tiff&quot;);//too slow

            imgOpt.TiffCompression = TiffCompression.CompressionRle;
            //wbRender = new WorkbookRender(wb, imgOpt);
            //wbRender.ToImage(Constants.destPath + @&quot;NetCoreTests\test_Cs_Rle.tiff&quot;);//too slow

            imgOpt.TiffCompression = TiffCompression.CompressionLZW;
            wbRender = new WorkbookRender(wb, imgOpt);
            wbRender.ToImage(Constants.destPath + @&quot;NetCoreTests\test_Cs_LZW.tiff&quot;);

            imgOpt.TiffCompression = TiffCompression.CompressionCCITT3;
            wbRender = new WorkbookRender(wb, imgOpt);
            wbRender.ToImage(Constants.destPath + @&quot;NetCoreTests\test_Cs_CCITT3.tiff&quot;);

            imgOpt.TiffCompression = TiffCompression.CompressionCCITT4;
            wbRender = new WorkbookRender(wb, imgOpt);
            wbRender.ToImage(Constants.destPath + @&quot;NetCoreTests\test_Cs_CCITT4.tiff&quot;);


        }
```

### See Also

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


