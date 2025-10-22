##SetTreatQuotePrefixAsValue Method
'SetTreatQuotePrefixAsValue method. Encapsulates the function that represents settreatquoteprefixasvalue in Go.'
## SetTreatQuotePrefixAsValue function
Indicates whether the leading single quote sign should be taken as part of the value of one cell.Default is true. If it is false, the leading single quote will be removed from corresponding cell's valueand Style.QuotePrefix will be set as true for the cell.
```go
func (instance *TxtLoadOptions) SetTreatQuotePrefixAsValue(value bool)  error
```
## Remarks
## See Also
* Class [TxtLoadOptions](../)
* Library [Aspose.Cells for Go](../../)
