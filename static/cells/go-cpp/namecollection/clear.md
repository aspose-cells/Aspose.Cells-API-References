##Clear Method
'Clear method. Encapsulates the function that represents clear in Go.'
## Clear function
Remove all defined names which are not referenced by the formulas and data source.If the defined name is referred, we only set Name.ReferTo as null and hide them.
```go
func (instance *NameCollection) Clear()  error
```
## Remarks
## See Also
* Class [NameCollection](../)
* Library [Aspose.Cells for Go](../../)
