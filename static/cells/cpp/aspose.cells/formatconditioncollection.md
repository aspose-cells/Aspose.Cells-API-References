##Aspose::Cells::FormatConditionCollection class
'Aspose::Cells::FormatConditionCollection class. Represents conditional formatting. The FormatConditions can contain up to three conditional formats in C++.'
## FormatConditionCollection class
Represents conditional formatting. The FormatConditions can contain up to three conditional formats.
```cpp
class FormatConditionCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(const CellArea\& cellArea, FormatConditionType type, OperatorType operatorType, const U16String\& formula1, const U16String\& formula2)](./add/) | Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. References to the other sheets are not allowed in the formulas of conditional formatting. |
| [Add(const CellArea\& cellArea, FormatConditionType type, OperatorType operatorType, const char16_t* formula1, const char16_t* formula2)](./add/) | Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. References to the other sheets are not allowed in the formulas of conditional formatting. |
| [AddArea(const CellArea\& cellArea)](./addarea/) | Adds a conditional formatted cell range. |
| [AddCondition(FormatConditionType type, OperatorType operatorType, const U16String\& formula1, const U16String\& formula2)](./addcondition/) | Adds a formatting condition. |
| [AddCondition(FormatConditionType type, OperatorType operatorType, const char16_t* formula1, const char16_t* formula2)](./addcondition/) | Adds a formatting condition. |
| [AddCondition(FormatConditionType type)](./addcondition/) | Add a format condition. |
| [FormatConditionCollection(FormatConditionCollection_Impl* impl)](./formatconditioncollection/) | Constructs from an implementation object. |
| [FormatConditionCollection(const FormatConditionCollection\& src)](./formatconditioncollection/) | Copy constructor. |
| [Get(int32_t index)](./get/) | Gets the formatting condition by index. |
| [GetCellArea(int32_t index)](./getcellarea/) | Gets the conditional formatted cell range by index. |
| [GetCount()](./getcount/) | Gets the count of the conditions. |
| [GetRangeCount()](./getrangecount/) | Gets count of conditionally formatted ranges. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const FormatConditionCollection\& src)](./operator_asm/) | operator= |
| [RemoveArea(int32_t index)](./removearea/) | Removes conditional formatted cell range by index. |
| [RemoveArea(int32_t startRow, int32_t startColumn, int32_t totalRows, int32_t totalColumns)](./removearea/) | Remove conditional formatting int the range. |
| [RemoveCondition(int32_t index)](./removecondition/) | Removes the formatting condition by index. |
| [~FormatConditionCollection()](./~formatconditioncollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Create a new Workbook.
Workbook workbook;
//Get the first worksheet.
Worksheet sheet = workbook.GetWorksheets().Get(0);
//Adds an empty conditional formatting
int index = sheet.GetConditionalFormattings().Add();
FormatConditionCollection fcs = sheet.GetConditionalFormattings().Get(index);
//Sets the conditional format range.
CellArea ca;
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 0;
ca.EndColumn = 0;
fcs.AddArea(ca);
ca = CellArea();
ca.StartRow = 1;
ca.EndRow = 1;
ca.StartColumn = 1;
ca.EndColumn = 1;
fcs.AddArea(ca);
//Adds condition.
int conditionIndex = fcs.AddCondition(FormatConditionType::CellValue, OperatorType::Between, u"=A2", u"100");
//Adds condition.
int conditionIndex2 = fcs.AddCondition(FormatConditionType::CellValue, OperatorType::Between, u"50", u"100");
//Sets the background color.
FormatCondition fc = fcs.Get(conditionIndex);
fc.GetStyle().SetBackgroundColor(Color{ 0xff, 0xff, 0, 0 });
//Saving the Excel file
workbook.Save(u"output.xls");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
