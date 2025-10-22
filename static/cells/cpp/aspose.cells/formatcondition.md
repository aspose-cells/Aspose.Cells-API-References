##Aspose::Cells::FormatCondition class
'Aspose::Cells::FormatCondition class. Represents conditional formatting condition in C++.'
## FormatCondition class
Represents conditional formatting condition.
```cpp
class FormatCondition
```
## Methods
| Method | Description |
| --- | --- |
| [FormatCondition(FormatCondition_Impl* impl)](./formatcondition/) | Constructs from an implementation object. |
| [FormatCondition(const FormatCondition\& src)](./formatcondition/) | Copy constructor. |
| [GetAboveAverage()](./getaboveaverage/) | Get the conditional formatting's "AboveAverage" instance. The default instance's rule highlights cells that are above the average for all values in the range. Valid only for type = [AboveAverage](../aboveaverage/). |
| [GetColorScale()](./getcolorscale/) | Get the conditional formatting's "ColorScale" instance. The default instance is a "green-yellow-red" 3[ColorScale](../colorscale/) . Valid only for type = [ColorScale](../colorscale/). |
| [GetDataBar()](./getdatabar/) | Get the conditional formatting's "DataBar" instance. The default instance's color is blue. Valid only for type is [DataBar](../databar/). |
| [GetFormula1(bool isR1C1, bool isLocal)](./getformula1/) | Gets the value or expression associated with this format condition. |
| [GetFormula1(bool isR1C1, bool isLocal, int32_t row, int32_t column)](./getformula1/) | Gets the value or expression of the conditional formatting of the cell. |
| [GetFormula1()](./getformula1/) | Gets and sets the value or expression associated with conditional formatting. |
| [GetFormula1(int32_t row, int32_t column)](./getformula1/) | Gets the formula of the conditional formatting of the cell. |
| [GetFormula2(bool isR1C1, bool isLocal)](./getformula2/) | Gets the value or expression associated with this format condition. |
| [GetFormula2(bool isR1C1, bool isLocal, int32_t row, int32_t column)](./getformula2/) | Gets the value or expression of the conditional formatting of the cell. |
| [GetFormula2()](./getformula2/) | Gets and sets the value or expression associated with conditional formatting. |
| [GetFormula2(int32_t row, int32_t column)](./getformula2/) | Gets the formula of the conditional formatting of the cell. |
| [GetIconSet()](./geticonset/) | Get the conditional formatting's "IconSet" instance. The default instance's IconSetType is TrafficLights31. Valid only for type = [IconSet](../iconset/). |
| [GetOperator()](./getoperator/) | Gets and sets the conditional format operator type. |
| [GetPriority()](./getpriority/) | The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values, where '1' is the highest priority. |
| [GetStopIfTrue()](./getstopiftrue/) | True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Excel 2007;. |
| [GetStyle()](./getstyle/) | Gets or setts style of conditional formatted cell ranges. |
| [GetText()](./gettext/) | The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, beginsWith and endsWith. The default value is null. |
| [GetTimePeriod()](./gettimeperiod/) | The applicable time period in a "date occurring…" conditional formatting rule. Valid only for type = timePeriod. The default value is [TimePeriodType.Today](../timeperiodtype/). |
| [GetTop10()](./gettop10/) | Get the conditional formatting's "Top10" instance. The default instance's rule highlights cells whose values fall in the top 10 bracket. Valid only for type is [Top10](../top10/). |
| [GetType()](./gettype/) | Gets and sets whether the conditional format Type. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const FormatCondition\& src)](./operator_asm/) | operator= |
| [SetFormula1(const U16String\& formula, bool isR1C1, bool isLocal)](./setformula1/) | Sets the value or expression associated with this format condition. |
| [SetFormula1(const char16_t* formula, bool isR1C1, bool isLocal)](./setformula1/) | Sets the value or expression associated with this format condition. |
| [SetFormula1(const U16String\& value)](./setformula1/) | Gets and sets the value or expression associated with conditional formatting. |
| [SetFormula1(const char16_t* value)](./setformula1/) | Gets and sets the value or expression associated with conditional formatting. |
| [SetFormula2(const U16String\& formula, bool isR1C1, bool isLocal)](./setformula2/) | Sets the value or expression associated with this format condition. |
| [SetFormula2(const char16_t* formula, bool isR1C1, bool isLocal)](./setformula2/) | Sets the value or expression associated with this format condition. |
| [SetFormula2(const U16String\& value)](./setformula2/) | Gets and sets the value or expression associated with conditional formatting. |
| [SetFormula2(const char16_t* value)](./setformula2/) | Gets and sets the value or expression associated with conditional formatting. |
| [SetFormulas(const U16String\& formula1, const U16String\& formula2, bool isR1C1, bool isLocal)](./setformulas/) | Sets the value or expression associated with this format condition. |
| [SetFormulas(const char16_t* formula1, const char16_t* formula2, bool isR1C1, bool isLocal)](./setformulas/) | Sets the value or expression associated with this format condition. |
| [SetOperator(OperatorType value)](./setoperator/) | Gets and sets the conditional format operator type. |
| [SetPriority(int32_t value)](./setpriority/) | The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values, where '1' is the highest priority. |
| [SetStopIfTrue(bool value)](./setstopiftrue/) | True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Excel 2007;. |
| [SetStyle(const Style\& value)](./setstyle/) | Gets or setts style of conditional formatted cell ranges. |
| [SetText(const U16String\& value)](./settext/) | The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, beginsWith and endsWith. The default value is null. |
| [SetText(const char16_t* value)](./settext/) | The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, beginsWith and endsWith. The default value is null. |
| [SetTimePeriod(TimePeriodType value)](./settimeperiod/) | The applicable time period in a "date occurring…" conditional formatting rule. Valid only for type = timePeriod. The default value is [TimePeriodType.Today](../timeperiodtype/). |
| [SetType(FormatConditionType value)](./settype/) | Gets and sets whether the conditional format Type. |
| [~FormatCondition()](./~formatcondition/) | Destructor. |
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
