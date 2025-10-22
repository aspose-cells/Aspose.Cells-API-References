##GetPageScale Method
'GetPageScale method. Encapsulates the function that represents getpagescale in Go.'
## GetPageScale function
Gets calculated page scale of the sheet.Returns the set scale if PageSetup.Zoom is set. Otherwise, returns the calculated scale according to PageSetup.FitToPagesWide and PageSetup.FitToPagesTall.
```go
func (instance *SheetRender) GetPageScale()  (float64,  error)
```
## Remarks
## See Also
* Class [SheetRender](../)
* Library [Aspose.Cells for Go](../../)
