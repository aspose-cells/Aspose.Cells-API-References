##SetImageResample Method
'SetImageResample method. Encapsulates the function that represents setimageresample in Go.'
## SetImageResample function
Sets desired PPI(pixels per inch) of resample images and jpeg quality.All images will be converted to JPEG with the specified quality setting,and images that are greater than the specified PPI (pixels per inch) will be resampled.
```go
func (instance *PdfSaveOptions) SetImageResample(desiredppi int32, jpegquality int32)  error
```
## Remarks
## See Also
* Class [PdfSaveOptions](../)
* Library [Aspose.Cells for Go](../../)
