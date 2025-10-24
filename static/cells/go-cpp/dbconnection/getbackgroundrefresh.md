##GetBackgroundRefresh Method
'GetBackgroundRefresh method. Encapsulates the function that represents getbackgroundrefresh in Go.'
## GetBackgroundRefresh function
Indicates whether the connection can be refreshed in the background (asynchronously).true if preferred usage of the connection is to refresh asynchronously in the background;false if preferred usage of the connection is to refresh synchronously in the foreground.
```go
func (instance *DBConnection) GetBackgroundRefresh()  (bool,  error)
```
## Remarks
## See Also
* Class [DBConnection](../)
* Library [Aspose.Cells for Go](../../)
