##PdfSaveOptions.SetImageResample
PdfSaveOptions method. Sets desired PPIpixels per inch of resample images and jpeg quality. All images will be converted to JPEG with the specified quality setting and images that are greater than the specified PPI pixels per inch will be resampled
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
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PdfSaveOptionsMethodSetImageResampleWithInt32Int32Demo
{
public static void Run()
{
Workbook wb = new Workbook("Book1.xlsx");
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.SetImageResample(96, 80);
wb.Save("output.pdf", pdfSaveOptions);
}
}
}
```
### See Also
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
