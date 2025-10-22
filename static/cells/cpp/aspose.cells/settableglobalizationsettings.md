##Aspose::Cells::SettableGlobalizationSettings class
'Aspose::Cells::SettableGlobalizationSettings class. Implementation of GlobalizationSettings that supports user to set/change pre-defined texts in C++.'
## SettableGlobalizationSettings class
Implementation of [GlobalizationSettings](../globalizationsettings/) that supports user to set/change pre-defined texts.
```cpp
class SettableGlobalizationSettings
```
## Methods
| Method | Description |
| --- | --- |
| [GetBooleanValueString(bool bv)](./getbooleanvaluestring/) | Gets the display string value for cell's boolean value. |
| [GetColumnSeparatorOfFormulaArray()](./getcolumnseparatorofformulaarray/) | Gets the separator for the items in array's row data in formula. |
| [GetCommentTitleName(CommentTitleType type)](./getcommenttitlename/) | Gets the locale dependent comment title name according to comment title type. |
| [GetErrorValueString(const U16String\& err)](./geterrorvaluestring/) | Gets the display string value for cell's error value. |
| [GetErrorValueString(const char16_t* err)](./geterrorvaluestring/) | Gets the display string value for cell's error value. |
| [GetGrandTotalName(ConsolidationFunction functionType)](./getgrandtotalname/) | Gets the grand total name of the function. |
| [GetListSeparator()](./getlistseparator/) | Gets the separator for list, parameters of function, ...etc. |
| [GetLocalBuiltInName(const U16String\& standardName)](./getlocalbuiltinname/) | Gets the locale dependent text for built-in [Name](../name/) according to given standard text. |
| [GetLocalBuiltInName(const char16_t* standardName)](./getlocalbuiltinname/) | Gets the locale dependent text for built-in [Name](../name/) according to given standard text. |
| [GetLocalFunctionName(const U16String\& standardName)](./getlocalfunctionname/) | Gets the locale dependent function name according to given standard function name. |
| [GetLocalFunctionName(const char16_t* standardName)](./getlocalfunctionname/) | Gets the locale dependent function name according to given standard function name. |
| [GetRowSeparatorOfFormulaArray()](./getrowseparatorofformulaarray/) | Gets the separator for rows in array data in formula. |
| [GetStandardBuiltInName(const U16String\& localName)](./getstandardbuiltinname/) | Gets the standard text of built-in [Name](../name/) according to given locale dependent text. |
| [GetStandardBuiltInName(const char16_t* localName)](./getstandardbuiltinname/) | Gets the standard text of built-in [Name](../name/) according to given locale dependent text. |
| [GetStandardFunctionName(const U16String\& localName)](./getstandardfunctionname/) | Gets the standard function name according to given locale dependent function name. |
| [GetStandardFunctionName(const char16_t* localName)](./getstandardfunctionname/) | Gets the standard function name according to given locale dependent function name. |
| [GetStandardHeaderFooterFontStyleName(const U16String\& localfontStyleName)](./getstandardheaderfooterfontstylename/) | Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name. |
| [GetStandardHeaderFooterFontStyleName(const char16_t* localfontStyleName)](./getstandardheaderfooterfontstylename/) | Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name. |
| [GetTableRowTypeOfAll()](./gettablerowtypeofall/) | Gets the type name of table rows that consists of all rows in referenced table. |
| [GetTableRowTypeOfCurrent()](./gettablerowtypeofcurrent/) | Gets the type name of table rows that consists of the current row in referenced table. |
| [GetTableRowTypeOfData()](./gettablerowtypeofdata/) | Gets the type name of table rows that consists of data region of referenced table. Default is "Data", so in formula "#Data" represents the data region of the table. |
| [GetTableRowTypeOfHeaders()](./gettablerowtypeofheaders/) | Gets the type name of table rows that consists of the table header. Default is "Headers", so in formula "#Headers" represents the table header. |
| [GetTableRowTypeOfTotals()](./gettablerowtypeoftotals/) | Gets the type name of table rows that consists of the total row of referenced table. |
| [GetTotalName(ConsolidationFunction functionType)](./gettotalname/) | Gets the total name of specific function. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SettableGlobalizationSettings\& src)](./operator_asm/) | operator= |
| [SetBooleanValueString(bool bv, const U16String\& name)](./setbooleanvaluestring/) | Sets the display string value for cell's boolean value. |
| [SetBooleanValueString(bool bv, const char16_t* name)](./setbooleanvaluestring/) | Sets the display string value for cell's boolean value. |
| [SetColumnSeparatorOfFormulaArray(char16_t c)](./setcolumnseparatorofformulaarray/) | Sets the separator for the items in array's row data in formula. |
| [SetCommentTitleName(CommentTitleType type, const U16String\& name)](./setcommenttitlename/) | Gets the locale dependent comment title name according to comment title type. |
| [SetCommentTitleName(CommentTitleType type, const char16_t* name)](./setcommenttitlename/) | Gets the locale dependent comment title name according to comment title type. |
| [SetGrandTotalName(ConsolidationFunction functionType, const U16String\& name)](./setgrandtotalname/) | Sets the grand total name of specific function. |
| [SetGrandTotalName(ConsolidationFunction functionType, const char16_t* name)](./setgrandtotalname/) | Sets the grand total name of specific function. |
| [SetListSeparator(char16_t c)](./setlistseparator/) | Sets the separator for list, parameters of function, ...etc. |
| [SetLocalBuiltInName(const U16String\& standardName, const U16String\& localName, bool bidirectional)](./setlocalbuiltinname/) | Sets the locale dependent text for the built-in name with given standard name text. |
| [SetLocalBuiltInName(const char16_t* standardName, const char16_t* localName, bool bidirectional)](./setlocalbuiltinname/) | Sets the locale dependent text for the built-in name with given standard name text. |
| [SetLocalFunctionName(const U16String\& standardName, const U16String\& localName, bool bidirectional)](./setlocalfunctionname/) | Sets the locale dependent function name corresponding to given standard function name. |
| [SetLocalFunctionName(const char16_t* standardName, const char16_t* localName, bool bidirectional)](./setlocalfunctionname/) | Sets the locale dependent function name corresponding to given standard function name. |
| [SetRowSeparatorOfFormulaArray(char16_t c)](./setrowseparatorofformulaarray/) | Sets the separator for rows in array data in formula. |
| [SetStandardBuiltInName(const U16String\& localName, const U16String\& standardName, bool bidirectional)](./setstandardbuiltinname/) | Sets the locale dependent function name according to given standard function name. |
| [SetStandardBuiltInName(const char16_t* localName, const char16_t* standardName, bool bidirectional)](./setstandardbuiltinname/) | Sets the locale dependent function name according to given standard function name. |
| [SetStandardFunctionName(const U16String\& localName, const U16String\& standardName, bool bidirectional)](./setstandardfunctionname/) | Sets the locale dependent function name according to given standard function name. |
| [SetStandardFunctionName(const char16_t* localName, const char16_t* standardName, bool bidirectional)](./setstandardfunctionname/) | Sets the locale dependent function name according to given standard function name. |
| [SetStandardHeaderFooterFontStyleName(const U16String\& localfontStyleName, const U16String\& standardName)](./setstandardheaderfooterfontstylename/) | Sets the locale dependent function name according to given standard function name. |
| [SetStandardHeaderFooterFontStyleName(const char16_t* localfontStyleName, const char16_t* standardName)](./setstandardheaderfooterfontstylename/) | Sets the locale dependent function name according to given standard function name. |
| [SettableGlobalizationSettings()](./settableglobalizationsettings/) | Default constructor. |
| [SettableGlobalizationSettings(SettableGlobalizationSettings_Impl* impl)](./settableglobalizationsettings/) | Constructs from an implementation object. |
| [SettableGlobalizationSettings(const SettableGlobalizationSettings\& src)](./settableglobalizationsettings/) | Copy constructor. |
| [SetTableRowTypeOfAll(const U16String\& name)](./settablerowtypeofall/) | Sets the type name of table rows that consists of all rows in referenced table. |
| [SetTableRowTypeOfAll(const char16_t* name)](./settablerowtypeofall/) | Sets the type name of table rows that consists of all rows in referenced table. |
| [SetTableRowTypeOfCurrent(const U16String\& name)](./settablerowtypeofcurrent/) | Sets the type name of table rows that consists of the current row in referenced table. |
| [SetTableRowTypeOfCurrent(const char16_t* name)](./settablerowtypeofcurrent/) | Sets the type name of table rows that consists of the current row in referenced table. |
| [SetTableRowTypeOfData(const U16String\& name)](./settablerowtypeofdata/) | Sets the type name of table rows that consists of data region of referenced table. |
| [SetTableRowTypeOfData(const char16_t* name)](./settablerowtypeofdata/) | Sets the type name of table rows that consists of data region of referenced table. |
| [SetTableRowTypeOfHeaders(const U16String\& name)](./settablerowtypeofheaders/) | Sets the type name of table rows that consists of the table header. |
| [SetTableRowTypeOfHeaders(const char16_t* name)](./settablerowtypeofheaders/) | Sets the type name of table rows that consists of the table header. |
| [SetTableRowTypeOfTotals(const U16String\& name)](./settablerowtypeoftotals/) | Sets the type name of table rows that consists of the total row of referenced table. |
| [SetTableRowTypeOfTotals(const char16_t* name)](./settablerowtypeoftotals/) | Sets the type name of table rows that consists of the total row of referenced table. |
| [SetTotalName(ConsolidationFunction functionType, const U16String\& name)](./settotalname/) | Sets the total name of specific function. |
| [SetTotalName(ConsolidationFunction functionType, const char16_t* name)](./settotalname/) | Sets the total name of specific function. |
| [~SettableGlobalizationSettings()](./~settableglobalizationsettings/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
