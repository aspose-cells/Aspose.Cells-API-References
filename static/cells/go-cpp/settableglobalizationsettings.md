##SettableGlobalizationSettings Class
'SettableGlobalizationSettings class. Encapsulates the object that represents settableglobalizationsettings in Go.'
## SettableGlobalizationSettings class
Implementation of GlobalizationSettings that supports user to set/change pre-defined texts.
```go
type SettableGlobalizationSettings struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewSettableGlobalizationSettings](./newsettableglobalizationsettings/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetTotalName](./gettotalname/) | Gets the total name of specific function. |
|[SetTotalName](./settotalname/) | Sets the total name of specific function. |
|[GetGrandTotalName](./getgrandtotalname/) | Gets the grand total name of the function. |
|[SetGrandTotalName](./setgrandtotalname/) | Sets the grand total name of specific function. |
|[GetTableRowTypeOfHeaders](./gettablerowtypeofheaders/) | Gets the type name of table rows that consists of the table header.Default is "Headers", so in formula "#Headers" represents the table header. |
|[SetTableRowTypeOfHeaders](./settablerowtypeofheaders/) | Sets the type name of table rows that consists of the table header. |
|[GetTableRowTypeOfData](./gettablerowtypeofdata/) | Gets the type name of table rows that consists of data region of referenced table.Default is "Data", so in formula "#Data" represents the data region of the table. |
|[SetTableRowTypeOfData](./settablerowtypeofdata/) | Sets the type name of table rows that consists of data region of referenced table. |
|[GetTableRowTypeOfAll](./gettablerowtypeofall/) | Gets the type name of table rows that consists of all rows in referenced table. |
|[SetTableRowTypeOfAll](./settablerowtypeofall/) | Sets the type name of table rows that consists of all rows in referenced table. |
|[GetTableRowTypeOfTotals](./gettablerowtypeoftotals/) | Gets the type name of table rows that consists of the total row of referenced table. |
|[SetTableRowTypeOfTotals](./settablerowtypeoftotals/) | Sets the type name of table rows that consists of the total row of referenced table. |
|[GetTableRowTypeOfCurrent](./gettablerowtypeofcurrent/) | Gets the type name of table rows that consists of the current row in referenced table. |
|[SetTableRowTypeOfCurrent](./settablerowtypeofcurrent/) | Sets the type name of table rows that consists of the current row in referenced table. |
|[GetErrorValueString](./geterrorvaluestring/) | Gets the display string value for cell's error value |
|[GetBooleanValueString](./getbooleanvaluestring/) | Gets the display string value for cell's boolean value |
|[SetBooleanValueString](./setbooleanvaluestring/) | Sets the display string value for cell's boolean value |
|[GetLocalFunctionName](./getlocalfunctionname/) | Gets the locale dependent function name according to given standard function name. |
|[SetLocalFunctionName](./setlocalfunctionname/) | Sets the locale dependent function name corresponding to given standard function name. |
|[GetStandardFunctionName](./getstandardfunctionname/) | Gets the standard function name according to given locale dependent function name. |
|[SetStandardFunctionName](./setstandardfunctionname/) | Sets the locale dependent function name according to given standard function name. |
|[GetLocalBuiltInName](./getlocalbuiltinname/) | Gets the locale dependent text for built-in Name according to given standard text. |
|[SetLocalBuiltInName](./setlocalbuiltinname/) | Sets the locale dependent text for the built-in name with given standard name text. |
|[GetStandardBuiltInName](./getstandardbuiltinname/) | Gets the standard text of built-in Name according to given locale dependent text. |
|[SetStandardBuiltInName](./setstandardbuiltinname/) | Sets the locale dependent function name according to given standard function name. |
|[GetListSeparator](./getlistseparator/) | Gets the separator for list, parameters of function, ...etc. |
|[SetListSeparator](./setlistseparator/) | Sets the separator for list, parameters of function, ...etc. |
|[GetRowSeparatorOfFormulaArray](./getrowseparatorofformulaarray/) | Gets the separator for rows in array data in formula. |
|[SetRowSeparatorOfFormulaArray](./setrowseparatorofformulaarray/) | Sets the separator for rows in array data in formula. |
|[GetColumnSeparatorOfFormulaArray](./getcolumnseparatorofformulaarray/) | Gets the separator for the items in array's row data in formula. |
|[SetColumnSeparatorOfFormulaArray](./setcolumnseparatorofformulaarray/) | Sets the separator for the items in array's row data in formula. |
|[GetStandardHeaderFooterFontStyleName](./getstandardheaderfooterfontstylename/) | Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name. |
|[SetStandardHeaderFooterFontStyleName](./setstandardheaderfooterfontstylename/) | Sets the locale dependent function name according to given standard function name. |
|[GetCommentTitleName](./getcommenttitlename/) | Gets the locale dependent comment title name according to comment title type. |
|[SetCommentTitleName](./setcommenttitlename/) | Gets the locale dependent comment title name according to comment title type. |
