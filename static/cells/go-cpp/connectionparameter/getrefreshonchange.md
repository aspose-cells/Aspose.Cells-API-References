##GetRefreshOnChange Method
'GetRefreshOnChange method. Encapsulates the function that represents getrefreshonchange in Go.'
## GetRefreshOnChange function
Flag indicating whether the query should automatically refresh when the contents of acell that provides the parameter value changes. If true, then external data is refreshedusing the new parameter value every time there's a change. If false, then external datais only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened).
```go
func (instance *ConnectionParameter) GetRefreshOnChange()  (bool,  error)
```
## Remarks
## See Also
* Class [ConnectionParameter](../)
* Library [Aspose.Cells for Go](../../)
