##Aspose::Cells::Pivot::PivotShowValuesSetting class
'Aspose::Cells::Pivot::PivotShowValuesSetting class. Represents the settings about showing values as when the ShowDataAs calculation is in use in C++.'
## PivotShowValuesSetting class
Represents the settings about showing values as when the ShowDataAs calculation is in use.
```cpp
class PivotShowValuesSetting
```
## Methods
| Method | Description |
| --- | --- |
| [GetBaseFieldIndex()](./getbasefieldindex/) | Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use. |
| [GetBaseItemIndex()](./getbaseitemindex/) | Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. |
| [GetBaseItemPositionType()](./getbaseitempositiontype/) | Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. Because [PivotItemPosition.Custom](../pivotitemposition/) is only for read,if you need to set [PivotItemPosition.Custom](../pivotitemposition/), please set PivotField.BaseItemIndex attribute. |
| [GetCalculationType()](./getcalculationtype/) | Represents how to show values of a data field in the pivot report. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PivotShowValuesSetting\& src)](./operator_asm/) | operator= |
| [PivotShowValuesSetting(PivotShowValuesSetting_Impl* impl)](./pivotshowvaluessetting/) | Constructs from an implementation object. |
| [PivotShowValuesSetting(const PivotShowValuesSetting\& src)](./pivotshowvaluessetting/) | Copy constructor. |
| [SetBaseFieldIndex(int32_t value)](./setbasefieldindex/) | Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use. |
| [SetBaseItemIndex(int32_t value)](./setbaseitemindex/) | Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. |
| [SetBaseItemPositionType(PivotItemPositionType value)](./setbaseitempositiontype/) | Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. Because [PivotItemPosition.Custom](../pivotitemposition/) is only for read,if you need to set [PivotItemPosition.Custom](../pivotitemposition/), please set PivotField.BaseItemIndex attribute. |
| [SetCalculationType(PivotFieldDataDisplayFormat value)](./setcalculationtype/) | Represents how to show values of a data field in the pivot report. |
| [~PivotShowValuesSetting()](./~pivotshowvaluessetting/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
