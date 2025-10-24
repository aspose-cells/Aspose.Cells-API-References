##GetDefaultFont Method
'GetDefaultFont method. Encapsulates the function that represents getdefaultfont in Go.'
## GetDefaultFont function
When characters in the Excel are Unicode and not be set with correct font in cell style,They may appear as block in pdf,image.Set the DefaultFont such as MingLiu or MS Gothic to show these characters.If this property is not set, Aspose.Cells will use system default font to show these unicode characters.
```go
func (instance *PclSaveOptions) GetDefaultFont()  (string,  error)
```
## Remarks
## See Also
* Class [PclSaveOptions](../)
* Library [Aspose.Cells for Go](../../)
