##SetBaseItemPositionType Method
'SetBaseItemPositionType method. Encapsulates the function that represents setbaseitempositiontype in Go.'
## SetBaseItemPositionType function
Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use.Valid only for data fields.Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom,please set PivotField.BaseItemIndex attribute.
```go
func (instance *PivotShowValuesSetting) SetBaseItemPositionType(value PivotItemPositionType)  error
```
## Remarks
## See Also
* Class [PivotShowValuesSetting](../)
* Library [Aspose.Cells for Go](../../)
