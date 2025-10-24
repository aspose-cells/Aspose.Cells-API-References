##Aspose::Cells::Pivot::PivotArea class
'Aspose::Cells::Pivot::PivotArea class. Presents the selected area of the PivotTable in C++.'
## PivotArea class
Presents the selected area of the [PivotTable](../pivottable/).
```cpp
class PivotArea
```
## Methods
| Method | Description |
| --- | --- |
| [GetAxisType()](./getaxistype/) | Gets and sets the region of the [PivotTable](../pivottable/) to which this rule applies. |
| [GetCellAreas()](./getcellareas/) | Gets cell areas of this pivot area. |
| [GetFilters()](./getfilters/) | Gets all filters for this [PivotArea](./). |
| [GetOnlyData()](./getonlydata/) | Indicates whether only the data values (in the data area of the view) for an item selection are selected and does not include the item labels. |
| [GetOnlyLabel()](./getonlylabel/) | Indicates whether only the data labels for an item selection are selected. |
| [GetRuleType()](./getruletype/) | Gets and sets the type of selection rule. |
| [IsColumnGrandIncluded()](./iscolumngrandincluded/) | Indicates whether the column grand total is included. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsOutline()](./isoutline/) | Indicates whether the rule refers to an area that is in outline mode. |
| [IsRowGrandIncluded()](./isrowgrandincluded/) | Indicates whether the row grand total is included. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PivotArea\& src)](./operator_asm/) | operator= |
| explicit [PivotArea(const PivotTable\& table)](./pivotarea/) | Presents the selected area of the [PivotTable](../pivottable/). |
| [PivotArea(PivotArea_Impl* impl)](./pivotarea/) | Constructs from an implementation object. |
| [PivotArea(const PivotArea\& src)](./pivotarea/) | Copy constructor. |
| [Select(PivotFieldType axisType, int32_t fieldPosition, PivotTableSelectionType selectionType)](./select/) | Select the area with filters. |
| [SelectField(PivotFieldType axisType, const U16String\& fieldName)](./selectfield/) | Select a field in the region as an area. |
| [SelectField(PivotFieldType axisType, const char16_t* fieldName)](./selectfield/) | Select a field in the region as an area. |
| [SelectField(PivotFieldType axisType, const PivotField\& field)](./selectfield/) | Select a field in the region as an area. |
| [SetAxisType(PivotFieldType value)](./setaxistype/) | Gets and sets the region of the [PivotTable](../pivottable/) to which this rule applies. |
| [SetIsColumnGrandIncluded(bool value)](./setiscolumngrandincluded/) | Indicates whether the column grand total is included. |
| [SetIsOutline(bool value)](./setisoutline/) | Indicates whether the rule refers to an area that is in outline mode. |
| [SetIsRowGrandIncluded(bool value)](./setisrowgrandincluded/) | Indicates whether the row grand total is included. |
| [SetOnlyData(bool value)](./setonlydata/) | Indicates whether only the data values (in the data area of the view) for an item selection are selected and does not include the item labels. |
| [SetOnlyLabel(bool value)](./setonlylabel/) | Indicates whether only the data labels for an item selection are selected. |
| [SetRuleType(PivotAreaType value)](./setruletype/) | Gets and sets the type of selection rule. |
| [~PivotArea()](./~pivotarea/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
