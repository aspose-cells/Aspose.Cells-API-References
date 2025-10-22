##PivotFormatCondition Class
'PivotFormatCondition class. Encapsulates the object that represents pivotformatcondition in Go.'
## PivotFormatCondition class
Represents a PivotTable Format Condition in PivotFormatCondition Collection.
```go
type PivotFormatCondition struct  {
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
|[AddDataAreaCondition_String](./adddataareacondition_string/) | Adds PivotTable conditional format limit in the data fields. |
|[AddDataAreaCondition_PivotField](./adddataareacondition_pivotfield/) | Adds PivotTable conditional format limit in the data fields. |
|[AddRowAreaCondition_String](./addrowareacondition_string/) | Adds PivotTable conditional format limit in the row fields. |
|[AddRowAreaCondition_PivotField](./addrowareacondition_pivotfield/) | Adds PivotTable conditional format limit in the row fields. |
|[AddColumnAreaCondition_String](./addcolumnareacondition_string/) | Adds PivotTable conditional format limit in the column fields. |
|[AddColumnAreaCondition_PivotField](./addcolumnareacondition_pivotfield/) | Adds PivotTable conditional format limit in the column fields. |
|[SetConditionalAreas](./setconditionalareas/) | Sets conditional areas of PivotFormatCondition object. |
|[GetScopeType](./getscopetype/) | Get and set scope type for the pivot table conditional format . |
|[SetScopeType](./setscopetype/) | Get and set scope type for the pivot table conditional format . |
|[GetRuleType](./getruletype/) | Get and set rule type for the pivot table condition format . |
|[SetRuleType](./setruletype/) | Get and set rule type for the pivot table condition format . |
|[GetFormatConditions](./getformatconditions/) | Get conditions for the pivot table conditional format . |
