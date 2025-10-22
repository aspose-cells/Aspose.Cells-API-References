##GetCheckWorkbookDefaultFont Method
'GetCheckWorkbookDefaultFont method. Encapsulates the function that represents getcheckworkbookdefaultfont in Go.'
## GetCheckWorkbookDefaultFont function
When characters in the Excel are Unicode and not be set with correct font in cell style,They may appear as block in pdf,image.Set this to true to try to use workbook's default font to show these characters first.
```go
func (instance *XpsSaveOptions) GetCheckWorkbookDefaultFont()  (bool,  error)
```
## Remarks
## See Also
* Class [XpsSaveOptions](../)
* Library [Aspose.Cells for Go](../../)
