##GetOnlyUseConnectionFile Method
'GetOnlyUseConnectionFile method. Encapsulates the function that represents getonlyuseconnectionfile in Go.'
## GetOnlyUseConnectionFile function
Indicates whether the spreadsheet application should always and only use theconnection information in the external connection file indicated by the odcFile attributewhen the connection is refreshed.  If false, then the spreadsheet applicationshould follow the procedure indicated by the reconnectionMethod attribute
```go
func (instance *WebQueryConnection) GetOnlyUseConnectionFile()  (bool,  error)
```
## Remarks
## See Also
* Class [WebQueryConnection](../)
* Library [Aspose.Cells for Go](../../)
