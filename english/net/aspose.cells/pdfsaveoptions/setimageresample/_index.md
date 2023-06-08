---
title: PdfSaveOptions.SetImageResample
second_title: Aspose.Cells for .NET API Reference
description: PdfSaveOptions method. Sets desired PPIpixels per inch of resample images and jpeg quality. All images will be converted to JPEG with the specified quality setting and images that are greater than the specified PPI pixels per inch will be resampled
type: docs
url: /net/aspose.cells/pdfsaveoptions/setimageresample/
---
## PdfSaveOptions.SetImageResample method

Sets desired PPI(pixels per inch) of resample images and jpeg quality. All images will be converted to JPEG with the specified quality setting, and images that are greater than the specified PPI (pixels per inch) will be resampled.

```csharp
public void SetImageResample(int desiredPPI, int jpegQuality)
```

| Parameter | Type | Description |
| --- | --- | --- |
| desiredPPI | Int32 | Desired pixels per inch. 220 high quality. 150 screen quality. 96 email quality. |
| jpegQuality | Int32 | 0 - 100% JPEG quality. |

### Examples

The following code sets desired PPI as 96 and jpeg quality as 80 for images in the output pdf.

```csharp
//load the source file with images.
Workbook wb = new Workbook("Book1.xlsx");

PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

//set desired PPI as 96 and jpeg quality as 80.
pdfSaveOptions.SetImageResample(96, 80);

wb.Save("output.pdf", pdfSaveOptions);
```

### See Also

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


