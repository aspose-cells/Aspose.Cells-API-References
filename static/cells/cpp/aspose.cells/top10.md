##Aspose::Cells::Top10 class
'Aspose::Cells::Top10 class. Describe the Top10 conditional formatting rule. This conditional formatting rule highlights cells whose values fall in the top N or bottom N bracket, as specified in C++.'
## Top10 class
Describe the [Top10](./) conditional formatting rule. This conditional formatting rule highlights cells whose values fall in the top N or bottom N bracket, as specified.
```cpp
class Top10
```
## Methods
| Method | Description |
| --- | --- |
| [GetRank()](./getrank/) | Get or set the value of "n" in a "top/bottom n" conditional formatting rule. If IsPercent is true, the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10. |
| [IsBottom()](./isbottom/) | Get or set whether a "top/bottom n" rule is a "bottom n" rule. Default value is false. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsPercent()](./ispercent/) | Get or set whether a "top/bottom n" rule is a "top/bottom n percent" rule. Default value is false. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Top10\& src)](./operator_asm/) | operator= |
| [SetIsBottom(bool value)](./setisbottom/) | Get or set whether a "top/bottom n" rule is a "bottom n" rule. Default value is false. |
| [SetIsPercent(bool value)](./setispercent/) | Get or set whether a "top/bottom n" rule is a "top/bottom n percent" rule. Default value is false. |
| [SetRank(int32_t value)](./setrank/) | Get or set the value of "n" in a "top/bottom n" conditional formatting rule. If IsPercent is true, the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10. |
| [Top10()](./top10/) | Default constructor. |
| [Top10(Top10_Impl* impl)](./top10/) | Constructs from an implementation object. |
| [Top10(const Top10\& src)](./top10/) | Copy constructor. |
| [~Top10()](./~top10/) | Destructor. |
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
//Adds an empty conditional formatting
int index = sheet.GetConditionalFormattings().Add();
FormatConditionCollection fcs = sheet.GetConditionalFormattings().Get(index);
//Sets the conditional format range.
CellArea ca = CellArea::CreateCellArea(0, 0, 10, 10);
fcs.AddArea(ca);
//Adds condition.
int conditionIndex = fcs.AddCondition(FormatConditionType::Top10, OperatorType::None, nullptr, nullptr);
//Sets the background color.
FormatCondition fc = fcs.Get(conditionIndex);
fc.GetStyle().SetBackgroundColor(Color{ 0xff, 0xff, 0, 0 });
Top10 top10 = fc.GetTop10();
//Set the Top N
top10.SetRank(5);
//Saving the Excel file
workbook.Save(u"output.xls");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
