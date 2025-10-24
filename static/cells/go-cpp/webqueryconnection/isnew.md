##IsNew Method
'IsNew method. Encapsulates the function that represents isnew in Go.'
## IsNew function
True if the connection has not been refreshed for the first time; otherwise, false.This state can happen when the user saves the file before a query has finished returning.
```go
func (instance *WebQueryConnection) IsNew()  (bool,  error)
```
## Remarks
## See Also
* Class [WebQueryConnection](../)
* Library [Aspose.Cells for Go](../../)
