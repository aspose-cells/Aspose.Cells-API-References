##SetHiddenColDisplayType Method
'SetHiddenColDisplayType method. Encapsulates the function that represents sethiddencoldisplaytype in Go.'
## SetHiddenColDisplayType function
Hidden column(the width of this column is 0) in excel,before save this into html format,if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output,if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden"
```go
func (instance *EbookSaveOptions) SetHiddenColDisplayType(value HtmlHiddenColDisplayType)  error
```
## Remarks
## See Also
* Class [EbookSaveOptions](../)
* Library [Aspose.Cells for Go](../../)
