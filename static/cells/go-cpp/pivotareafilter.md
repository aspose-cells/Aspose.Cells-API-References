##PivotAreaFilter Class
'PivotAreaFilter class. Encapsulates the object that represents pivotareafilter in Go.'
## PivotAreaFilter class
Represents the filter of <see cref="PivotArea"/> for <see cref="PivotTable"/>.
```go
type PivotAreaFilter struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewPivotAreaFilter](./newpivotareafilter/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[IsSubtotalSet](./issubtotalset/) | Gets which subtotal is set for this filter. |
|[SetSubtotals](./setsubtotals/) | Subtotal for the filter. |
|[GetSelected](./getselected/) | Indicates whether this field has selection.Only works when the PivotTable is in Outline view. |
|[SetSelected](./setselected/) | Indicates whether this field has selection.Only works when the PivotTable is in Outline view. |
