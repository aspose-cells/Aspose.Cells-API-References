##Aspose::Cells::GlobalizationSettings class
'Aspose::Cells::GlobalizationSettings class. Represents the globalization settings in C++.'
## GlobalizationSettings class
Represents the globalization settings.
```cpp
class GlobalizationSettings
```
## Methods
| Method | Description |
| --- | --- |
| virtual [Compare(const U16String\& v1, const U16String\& v2, bool ignoreCase)](./compare/) | Compares two string values according to certain collation rules. |
| virtual [Compare(const char16_t* v1, const char16_t* v2, bool ignoreCase)](./compare/) | Compares two string values according to certain collation rules. |
| virtual [GetBooleanValueString(bool bv)](./getbooleanvaluestring/) | Gets the display string value for cell's boolean value. |
| [GetChartSettings()](./getchartsettings/) | Gets the globalization settings for Chart. |
| virtual [GetColumnSeparatorOfFormulaArray()](./getcolumnseparatorofformulaarray/) | Gets the separator for the items in array's row data in formula. |
| virtual [GetCommentTitleName(CommentTitleType type)](./getcommenttitlename/) | Gets the locale dependent comment title name according to comment title type. |
| virtual [GetDefaultSheetName()](./getdefaultsheetname/) | Gets the default sheet name for adding worksheet automatically. Default is "Sheet". |
| virtual [GetErrorValueString(const U16String\& err)](./geterrorvaluestring/) | Gets the display string value for cell's error value. |
| virtual [GetErrorValueString(const char16_t* err)](./geterrorvaluestring/) | Gets the display string value for cell's error value. |
| virtual [GetGrandTotalName(ConsolidationFunction functionType)](./getgrandtotalname/) | Gets the grand total name of the function. |
| virtual [GetListSeparator()](./getlistseparator/) | Gets the separator for list, parameters of function, ...etc. |
| virtual [GetLocalBuiltInName(const U16String\& standardName)](./getlocalbuiltinname/) | Gets the locale dependent text for built-in [Name](../name/) according to given standard text. |
| virtual [GetLocalBuiltInName(const char16_t* standardName)](./getlocalbuiltinname/) | Gets the locale dependent text for built-in [Name](../name/) according to given standard text. |
| virtual [GetLocalFunctionName(const U16String\& standardName)](./getlocalfunctionname/) | Gets the locale dependent function name according to given standard function name. |
| virtual [GetLocalFunctionName(const char16_t* standardName)](./getlocalfunctionname/) | Gets the locale dependent function name according to given standard function name. |
| [GetPivotSettings()](./getpivotsettings/) | Gets the globalization settings for pivot table. |
| virtual [GetRowSeparatorOfFormulaArray()](./getrowseparatorofformulaarray/) | Gets the separator for rows in array data in formula. |
| virtual [GetStandardBuiltInName(const U16String\& localName)](./getstandardbuiltinname/) | Gets the standard text of built-in [Name](../name/) according to given locale dependent text. |
| virtual [GetStandardBuiltInName(const char16_t* localName)](./getstandardbuiltinname/) | Gets the standard text of built-in [Name](../name/) according to given locale dependent text. |
| virtual [GetStandardFunctionName(const U16String\& localName)](./getstandardfunctionname/) | Gets the standard function name according to given locale dependent function name. |
| virtual [GetStandardFunctionName(const char16_t* localName)](./getstandardfunctionname/) | Gets the standard function name according to given locale dependent function name. |
| virtual [GetStandardHeaderFooterFontStyleName(const U16String\& localfontStyleName)](./getstandardheaderfooterfontstylename/) | Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name. |
| virtual [GetStandardHeaderFooterFontStyleName(const char16_t* localfontStyleName)](./getstandardheaderfooterfontstylename/) | Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name. |
| virtual [GetTableRowTypeOfAll()](./gettablerowtypeofall/) | Gets the type name of table rows that consists of all rows in referenced table. Default is "All", so in formula "#All" represents all rows in referenced table. |
| virtual [GetTableRowTypeOfCurrent()](./gettablerowtypeofcurrent/) | Gets the type name of table rows that consists of the current row in referenced table. Default is "This Row", so in formula "#This Row" represents the current row in referenced table. |
| virtual [GetTableRowTypeOfData()](./gettablerowtypeofdata/) | Gets the type name of table rows that consists of data region of referenced table. Default is "Data", so in formula "#Data" represents the data region of the table. |
| virtual [GetTableRowTypeOfHeaders()](./gettablerowtypeofheaders/) | Gets the type name of table rows that consists of the table header. Default is "Headers", so in formula "#Headers" represents the table header. |
| virtual [GetTableRowTypeOfTotals()](./gettablerowtypeoftotals/) | Gets the type name of table rows that consists of the total row of referenced table. Default is "Totals", so in formula "#Totals" represents the total row of referenced table. |
| virtual [GetTotalName(ConsolidationFunction functionType)](./gettotalname/) | Gets the total name of the function. |
| [GlobalizationSettings()](./globalizationsettings/) | Default constructor. |
| [GlobalizationSettings(const GlobalizationSettings\& src)](./globalizationsettings/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const GlobalizationSettings\& src)](./operator_asm/) |  |
| [SetChartSettings(ChartGlobalizationSettings* value)](./setchartsettings/) | Sets the globalization settings for Chart. |
| [SetPivotSettings(PivotGlobalizationSettings* value)](./setpivotsettings/) | Sets the globalization settings for pivot table. |
| [~GlobalizationSettings()](./~globalizationsettings/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
