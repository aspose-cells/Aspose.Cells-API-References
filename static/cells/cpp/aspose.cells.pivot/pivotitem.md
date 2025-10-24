##Aspose::Cells::Pivot::PivotItem class
'Aspose::Cells::Pivot::PivotItem class. Represents a item in a PivotField report in C++.'
## PivotItem class
Represents a item in a [PivotField](../pivotfield/) report.
```cpp
class PivotItem
```
## Methods
| Method | Description |
| --- | --- |
| [GetDateTimeValue()](./getdatetimevalue/) | Gets the date time value of the pivot item If the value is null ,it will return DateTime.MinValue. |
| [GetDoubleValue()](./getdoublevalue/) | Gets the double value of the pivot item If the value is null or not number ,it will return 0. |
| [GetFormula()](./getformula/) | Gets the formula of this calculated item. Only works when this item is calculated item. |
| [GetIndex()](./getindex/) | Gets the index of the pivot item in cache field. |
| [GetName()](./getname/) | Gets the name of the pivot item. |
| [GetPosition()](./getposition/) | Specifying the position index in all the PivotItems,not the PivotItems under the same parent node. |
| [GetPositionInSameParentNode()](./getpositioninsameparentnode/) | Specifying the position index in the PivotItems under the same parent node. |
| [GetStringValue()](./getstringvalue/) | Gets the string value of the pivot item If the value is null, it will return "". |
| [GetValue()](./getvalue/) | Gets the value of the pivot item. |
| [IsCalculatedItem()](./iscalculateditem/) | Indicates whether this pivot item is a calculated formula item. |
| [IsDetailHidden()](./isdetailhidden/) | Gets and sets whether the detail of this pivot item is hidden. |
| [IsHidden()](./ishidden/) | Gets and Sets whether the pivot item is hidden. |
| [IsMissing()](./ismissing/) | Indicates whether the item is removed from the data source. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [Move(int32_t count, bool isSameParent)](./move/) | Moves the item up or down. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PivotItem\& src)](./operator_asm/) | operator= |
| [PivotItem(PivotItem_Impl* impl)](./pivotitem/) | Constructs from an implementation object. |
| [PivotItem(const PivotItem\& src)](./pivotitem/) | Copy constructor. |
| [SetIndex(int32_t value)](./setindex/) | Gets the index of the pivot item in cache field. |
| [SetIsDetailHidden(bool value)](./setisdetailhidden/) | Gets and sets whether the detail of this pivot item is hidden. |
| [SetIsHidden(bool value)](./setishidden/) | Gets and Sets whether the pivot item is hidden. |
| [SetName(const U16String\& value)](./setname/) | Gets the name of the pivot item. |
| [SetName(const char16_t* value)](./setname/) | Gets the name of the pivot item. |
| [SetPosition(int32_t value)](./setposition/) | Specifying the position index in all the PivotItems,not the PivotItems under the same parent node. |
| [SetPositionInSameParentNode(int32_t value)](./setpositioninsameparentnode/) | Specifying the position index in the PivotItems under the same parent node. |
| [~PivotItem()](./~pivotitem/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
