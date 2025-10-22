##PivotConditionalFormat Class
'PivotConditionalFormat class. Encapsulates the object that represents pivotconditionalformat in Go.'
## PivotConditionalFormat class
Represents a PivotTable Format Condition in PivotFormatCondition Collection.
```go
type PivotConditionalFormat struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetCellAreas](./getcellareas/) | Gets all cell areas where this conditional format applies to. |
|[GetPivotAreas](./getpivotareas/) | Gets all pivot areas. |
|[AddCellArea](./addcellarea/) | Adds an area based on pivot table view. |
|[ApplyTo](./applyto/) | Applies the conditional format to range.Only for the data region. |
|[AddFieldArea_PivotFieldType_String](./addfieldarea_pivotfieldtype_string/) | Adds an area of pivot field. |
|[AddFieldArea_PivotFieldType_PivotField](./addfieldarea_pivotfieldtype_pivotfield/) | Adds an area of pivot field. |
|[GetFormatConditions](./getformatconditions/) | Get conditions for the pivot table conditional format . |
|[GetScopeType](./getscopetype/) | Get and set scope type for the pivot table conditional format . |
|[SetScopeType](./setscopetype/) | Get and set scope type for the pivot table conditional format . |
|[GetRuleType](./getruletype/) | Get and set rule type for the pivot table condition format . |
|[SetRuleType](./setruletype/) | Get and set rule type for the pivot table condition format . |
