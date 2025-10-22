##GetEditWebPage Method
'GetEditWebPage method. Encapsulates the function that represents geteditwebpage in Go.'
## GetEditWebPage function
The URL of the user-facing web page showing the web query data. This URL is persistedin the case that sourceData="true" and url has been redirected to reference an XML file.Then the user-facing page can be shown in the UI, and the XML data can be retrievedbehind the scenes.
```go
func (instance *WebQueryConnection) GetEditWebPage()  (string,  error)
```
## Remarks
## See Also
* Class [WebQueryConnection](../)
* Library [Aspose.Cells for Go](../../)
