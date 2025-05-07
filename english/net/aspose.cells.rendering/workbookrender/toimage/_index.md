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
// Called: wbRender.ToImage(Constants.destPath + @"NetCoreTests\test_Cs_LZW.tiff");
[Test]
        public void Method_String_()
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
// Called: wr.ToImage(i, Constants.checkPath + "License/PluginImage"
private void Method_String_(Workbook wb, string fnId)
        {
            WorkbookRender wr = new WorkbookRender(wb, new ImageOrPrintOptions()
            { OnePagePerSheet = true });
            for (int i = 0; i < wr.PageCount; i++)
            {
                wr.ToImage(i, Constants.checkPath + "License/PluginImage"
                    + fnId + "_" + i + ".png");
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

### See Also

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


