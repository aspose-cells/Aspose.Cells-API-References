---
title: WorkbookRender.WorkbookRender
second_title: Aspose.Cells for .NET API Reference
description: WorkbookRender constructor. The construct of WorkbookRender
type: docs
url: /net/aspose.cells.rendering/workbookrender/workbookrender/
---
## WorkbookRender constructor

The construct of WorkbookRender

```csharp
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | Indicate which workbook to be rendered. |
| options | ImageOrPrintOptions | ImageOrPrintOptions contains some property of output image |

### Examples

```csharp
// Called: wbRender = new WorkbookRender(wb, imgOpt);
[Test]
        public void WorkbookRender_Constructor()
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

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


