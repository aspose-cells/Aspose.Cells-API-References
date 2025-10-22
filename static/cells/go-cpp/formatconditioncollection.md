##FormatConditionCollection Class
'FormatConditionCollection class. Encapsulates the object that represents formatconditioncollection in Go.'
## FormatConditionCollection class
Represents conditional formatting.The FormatConditions can contain up to three conditional formats.
```go
type FormatConditionCollection struct  {
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
|[Add](./add/) | Adds a formatting condition and effected cell rang to the FormatConditionsThe FormatConditions can contain up to three conditional formats.References to the other sheets are not allowed in the formulas of conditional formatting. |
|[AddArea](./addarea/) | Adds a conditional formatted cell range. |
|[AddCondition_FormatConditionType_OperatorType_String_String](./addcondition_formatconditiontype_operatortype_string_string/) | Adds a formatting condition. |
|[AddCondition_FormatConditionType](./addcondition_formatconditiontype/) | Add a format condition. |
|[GetCount](./getcount/) | Gets the count of the conditions. |
|[GetRangeCount](./getrangecount/) | Gets count of conditionally formatted ranges. |
|[Get](./get/) | Gets the formatting condition by index. |
|[GetCellArea](./getcellarea/) | Gets the conditional formatted cell range by index. |
|[RemoveArea_Int](./removearea_int/) | Removes conditional formatted cell range by index. |
|[RemoveArea_Int_Int_Int_Int](./removearea_int_int_int_int/) | Remove conditional formatting int the range. |
|[RemoveCondition](./removecondition/) | Removes the formatting condition by index. |
