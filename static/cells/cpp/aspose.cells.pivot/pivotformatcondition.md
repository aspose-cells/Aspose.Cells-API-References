##Aspose::Cells::Pivot::PivotFormatCondition class
'Aspose::Cells::Pivot::PivotFormatCondition class. Represents a PivotTable Format Condition in PivotFormatCondition Collection in C++.'
## PivotFormatCondition class
Represents a [PivotTable](../pivottable/) Format Condition in [PivotFormatCondition](./) Collection.
>Deprecated
>
>Use PivotConditionalFormat class instead.
```cpp
class PivotFormatCondition
```
## Methods
| Method | Description |
| --- | --- |
| [AddColumnAreaCondition(const U16String\& fieldName)](./addcolumnareacondition/) | Adds [PivotTable](../pivottable/) conditional format limit in the column fields. |
| [AddColumnAreaCondition(const char16_t* fieldName)](./addcolumnareacondition/) | Adds [PivotTable](../pivottable/) conditional format limit in the column fields. |
| [AddColumnAreaCondition(const PivotField\& columnField)](./addcolumnareacondition/) | Adds [PivotTable](../pivottable/) conditional format limit in the column fields. |
| [AddDataAreaCondition(const U16String\& fieldName)](./adddataareacondition/) | Adds [PivotTable](../pivottable/) conditional format limit in the data fields. |
| [AddDataAreaCondition(const char16_t* fieldName)](./adddataareacondition/) | Adds [PivotTable](../pivottable/) conditional format limit in the data fields. |
| [AddDataAreaCondition(const PivotField\& dataField)](./adddataareacondition/) | Adds [PivotTable](../pivottable/) conditional format limit in the data fields. |
| [AddRowAreaCondition(const U16String\& fieldName)](./addrowareacondition/) | Adds [PivotTable](../pivottable/) conditional format limit in the row fields. |
| [AddRowAreaCondition(const char16_t* fieldName)](./addrowareacondition/) | Adds [PivotTable](../pivottable/) conditional format limit in the row fields. |
| [AddRowAreaCondition(const PivotField\& rowField)](./addrowareacondition/) | Adds [PivotTable](../pivottable/) conditional format limit in the row fields. |
| [GetFormatConditions()](./getformatconditions/) | Get conditions for the pivot table conditional format . |
| [GetRuleType()](./getruletype/) | Get and set rule type for the pivot table condition format . |
| [GetScopeType()](./getscopetype/) | Get and set scope type for the pivot table conditional format . |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PivotFormatCondition\& src)](./operator_asm/) | operator= |
| [PivotFormatCondition(PivotFormatCondition_Impl* impl)](./pivotformatcondition/) | Constructs from an implementation object. |
| [PivotFormatCondition(const PivotFormatCondition\& src)](./pivotformatcondition/) | Copy constructor. |
| [SetConditionalAreas()](./setconditionalareas/) | Sets conditional areas of [PivotFormatCondition](./) object. |
| [SetRuleType(PivotConditionFormatRuleType value)](./setruletype/) | Get and set rule type for the pivot table condition format . |
| [SetScopeType(PivotConditionFormatScopeType value)](./setscopetype/) | Get and set scope type for the pivot table conditional format . |
| [~PivotFormatCondition()](./~pivotformatcondition/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Remarks
NOTE: This class is now obsolete. Instead, please use [PivotConditionalFormat](../pivotconditionalformat/) class. This method will be removed 12 months later since December 2024. **Aspose** apologizes for any inconvenience you may have experienced.
## See Also
* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
