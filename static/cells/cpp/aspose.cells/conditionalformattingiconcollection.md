##Aspose::Cells::ConditionalFormattingIconCollection class
'Aspose::Cells::ConditionalFormattingIconCollection class. Represents a collection of ConditionalFormattingIcon objects in C++.'
## ConditionalFormattingIconCollection class
Represents a collection of [ConditionalFormattingIcon](../conditionalformattingicon/) objects.
```cpp
class ConditionalFormattingIconCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(IconSetType type, int32_t index)](./add/) | Adds [ConditionalFormattingIcon](../conditionalformattingicon/) object. |
| [Add(const ConditionalFormattingIcon\& cficon)](./add/) | Adds [ConditionalFormattingIcon](../conditionalformattingicon/) object. |
| [ConditionalFormattingIconCollection(ConditionalFormattingIconCollection_Impl* impl)](./conditionalformattingiconcollection/) | Constructs from an implementation object. |
| [ConditionalFormattingIconCollection(const ConditionalFormattingIconCollection\& src)](./conditionalformattingiconcollection/) | Copy constructor. |
| [Get(int32_t index)](./get/) | Gets the [ConditionalFormattingIcon](../conditionalformattingicon/) element at the specified index. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ConditionalFormattingIconCollection\& src)](./operator_asm/) | operator= |
| [~ConditionalFormattingIconCollection()](./~conditionalformattingiconcollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
Worksheet sheet = workbook.GetWorksheets().Get(0);
//Get Conditional Formatting
ConditionalFormattingCollection cformattings = sheet.GetConditionalFormattings();
//Adds an empty conditional formatting
int index = cformattings.Add();
//Get newly added Conditional formatting
FormatConditionCollection fcs = cformattings.Get(index);
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
//Sets condition
int idx = fcs.AddCondition(FormatConditionType::IconSet);
FormatCondition cond = fcs.Get(idx);
//Sets condition's type
cond.GetIconSet().SetType(IconSetType::ArrowsGray3);
//Add custom iconset condition.
ConditionalFormattingIcon cfIcon = cond.GetIconSet().GetCfIcons().Get(0);
cfIcon.SetType(IconSetType::Arrows3);
cfIcon.SetIndex(0);
ConditionalFormattingIcon cfIcon1 = cond.GetIconSet().GetCfIcons().Get(1);
cfIcon1.SetType(IconSetType::ArrowsGray3);
cfIcon1.SetIndex(1);
ConditionalFormattingIcon cfIcon2 = cond.GetIconSet().GetCfIcons().Get(2);
cfIcon2.SetType(IconSetType::Boxes5);
cfIcon2.SetIndex(2);
//Saving the Excel file
workbook.Save(u"output.xls");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
