##GetTreatQuotePrefixAsValue Method
'GetTreatQuotePrefixAsValue method. Encapsulates the function that represents gettreatquoteprefixasvalue in Go.'
## GetTreatQuotePrefixAsValue function
Indicates whether the leading single quote sign should be taken as part of the value of one cell.Default is true. If it is false, the leading single quote will be removed from corresponding cell's valueand Style.QuotePrefix will be set as true for the cell.
```go
func (instance *TxtLoadOptions) GetTreatQuotePrefixAsValue()  (bool,  error)
```
## Remarks
## See Also
* Class [TxtLoadOptions](../)
* Library [Aspose.Cells for Go](../../)
