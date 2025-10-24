##GetHiddenRowDisplayType Method
'GetHiddenRowDisplayType method. Encapsulates the function that represents gethiddenrowdisplaytype in Go.'
## GetHiddenRowDisplayType function
Hidden row(the height of this row is 0) in excel,before save this into html format,if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output,if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden"
```go
func (instance *EbookSaveOptions) GetHiddenRowDisplayType()  (HtmlHiddenRowDisplayType,  error)
```
## Remarks
## See Also
* Class [EbookSaveOptions](../)
* Library [Aspose.Cells for Go](../../)
