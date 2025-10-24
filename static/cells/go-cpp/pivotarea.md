##PivotArea Class
'PivotArea class. Encapsulates the object that represents pivotarea in Go.'
## PivotArea class
Presents the selected area of the PivotTable.
```go
type PivotArea struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewPivotArea](./newpivotarea/) | Presents the selected area of the PivotTable. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetFilters](./getfilters/) | Gets all filters for this PivotArea. |
|[Select](./select/) | Select the area with filters. |
|[SelectField_PivotFieldType_String](./selectfield_pivotfieldtype_string/) | Select a field in the region as an area. |
|[SelectField_PivotFieldType_PivotField](./selectfield_pivotfieldtype_pivotfield/) | Select a field in the region as an area. |
|[GetOnlyData](./getonlydata/) | Indicates whether only the data values (in the data area of the view) for an itemselection are selected and does not include the item labels. |
|[SetOnlyData](./setonlydata/) | Indicates whether only the data values (in the data area of the view) for an itemselection are selected and does not include the item labels. |
|[GetOnlyLabel](./getonlylabel/) | Indicates whether only the data labels for an item selection are selected. |
|[SetOnlyLabel](./setonlylabel/) | Indicates whether only the data labels for an item selection are selected. |
|[IsRowGrandIncluded](./isrowgrandincluded/) | Indicates whether the row grand total is included. |
|[SetIsRowGrandIncluded](./setisrowgrandincluded/) | Indicates whether the row grand total is included. |
|[IsColumnGrandIncluded](./iscolumngrandincluded/) | Indicates whether the column grand total is included. |
|[SetIsColumnGrandIncluded](./setiscolumngrandincluded/) | Indicates whether the column grand total is included. |
|[GetAxisType](./getaxistype/) | Gets and sets the region of the PivotTable to which this rule applies. |
|[SetAxisType](./setaxistype/) | Gets and sets the region of the PivotTable to which this rule applies. |
|[GetRuleType](./getruletype/) | Gets and sets the type of selection rule. |
|[SetRuleType](./setruletype/) | Gets and sets the type of selection rule. |
|[IsOutline](./isoutline/) | Indicates whether the rule refers to an area that is in outline mode. |
|[SetIsOutline](./setisoutline/) | Indicates whether the rule refers to an area that is in outline mode. |
|[GetCellAreas](./getcellareas/) | Gets cell areas of this pivot area. |
