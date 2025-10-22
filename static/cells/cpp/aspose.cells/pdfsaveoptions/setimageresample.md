##Aspose::Cells::PdfSaveOptions::SetImageResample method
'Aspose::Cells::PdfSaveOptions::SetImageResample method. Sets desired PPI(pixels per inch) of resample images and jpeg quality. All images will be converted to JPEG with the specified quality setting, and images that are greater than the specified PPI (pixels per inch) will be resampled in C++.'
## PdfSaveOptions::SetImageResample method
Sets desired PPI(pixels per inch) of resample images and jpeg quality. All images will be converted to JPEG with the specified quality setting, and images that are greater than the specified PPI (pixels per inch) will be resampled.
```cpp
void Aspose::Cells::PdfSaveOptions::SetImageResample(int32_t desiredPPI, int32_t jpegQuality)
```
| Parameter | Type | Description |
| --- | --- | --- |
| desiredPPI | int32_t | Desired pixels per inch. 220 high quality. 150 screen quality. 96 email quality. |
| jpegQuality | int32_t | 0 - 100% JPEG quality. |
## Examples
```cpp
Aspose::Cells::Startup();
//The following code sets desired PPI as 96 and jpeg quality as 80 for images in the output pdf.
//load the source file with images.
Workbook wb(u"Book1.xlsx");
PdfSaveOptions pdfSaveOptions;
//set desired PPI as 96 and jpeg quality as 80.
pdfSaveOptions.SetImageResample(96, 80);
wb.Save(u"output.pdf", pdfSaveOptions);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [PdfSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
