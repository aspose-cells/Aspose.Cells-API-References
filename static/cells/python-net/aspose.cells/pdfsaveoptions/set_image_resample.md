##set_image_resample method
## set_image_resample(self, desired_ppi, jpeg_quality) {#int-int}
Sets desired PPI(pixels per inch) of resample images and jpeg quality.
All images will be converted to JPEG with the specified quality setting,
and images that are greater than the specified PPI (pixels per inch) will be resampled.
```python
def set_image_resample(self, desired_ppi, jpeg_quality):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| desired_ppi | int | Desired pixels per inch. 220 high quality. 150 screen quality. 96 email quality. |
| jpeg_quality | int | 0 - 100% JPEG quality. |
### Example
The following code sets desired PPI as 96 and jpeg quality as 80 for images in the output pdf.
```python
from aspose.cells import PdfSaveOptions, Workbook
# load the source file with images.
wb = Workbook("Book1.xlsx")
pdfSaveOptions = PdfSaveOptions()
# set desired PPI as 96 and jpeg quality as 80.
pdfSaveOptions.set_image_resample(96, 80)
wb.save("output.pdf", pdfSaveOptions)
```
### See Also
* module [`aspose.cells`](../../)
* class [`PdfSaveOptions`](/cells/python-net/aspose.cells/pdfsaveoptions)
