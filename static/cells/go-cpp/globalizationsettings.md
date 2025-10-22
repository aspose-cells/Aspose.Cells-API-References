##GlobalizationSettings Class
'GlobalizationSettings class. Encapsulates the object that represents globalizationsettings in Go.'
## GlobalizationSettings class
Represents the globalization settings.
```go
type GlobalizationSettings struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewGlobalizationSettings](./newglobalizationsettings/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetChartSettings](./getchartsettings/) | Gets the globalization settings for Chart. |
|[SetChartSettings](./setchartsettings/) | Sets the globalization settings for Chart. |
|[GetPivotSettings](./getpivotsettings/) | Gets the globalization settings for pivot table. |
|[SetPivotSettings](./setpivotsettings/) | Sets the globalization settings for pivot table. |
|[GetTotalName](./gettotalname/) | Gets the total name of the function. |
|[GetGrandTotalName](./getgrandtotalname/) | Gets the grand total name of the function. |
|[GetDefaultSheetName](./getdefaultsheetname/) | Gets the default sheet name for adding worksheet automatically.Default is "Sheet". |
|[GetTableRowTypeOfHeaders](./gettablerowtypeofheaders/) | Gets the type name of table rows that consists of the table header.Default is "Headers", so in formula "#Headers" represents the table header. |
|[GetTableRowTypeOfData](./gettablerowtypeofdata/) | Gets the type name of table rows that consists of data region of referenced table.Default is "Data", so in formula "#Data" represents the data region of the table. |
|[GetTableRowTypeOfAll](./gettablerowtypeofall/) | Gets the type name of table rows that consists of all rows in referenced table.Default is "All", so in formula "#All" represents all rows in referenced table. |
|[GetTableRowTypeOfTotals](./gettablerowtypeoftotals/) | Gets the type name of table rows that consists of the total row of referenced table.Default is "Totals", so in formula "#Totals" represents the total row of referenced table. |
|[GetTableRowTypeOfCurrent](./gettablerowtypeofcurrent/) | Gets the type name of table rows that consists of the current row in referenced table.Default is "This Row", so in formula "#This Row" represents the current row in referenced table. |
|[GetErrorValueString](./geterrorvaluestring/) | Gets the display string value for cell's error value |
|[GetBooleanValueString](./getbooleanvaluestring/) | Gets the display string value for cell's boolean value |
|[GetLocalFunctionName](./getlocalfunctionname/) | Gets the locale dependent function name according to given standard function name. |
|[GetStandardFunctionName](./getstandardfunctionname/) | Gets the standard function name according to given locale dependent function name. |
|[GetLocalBuiltInName](./getlocalbuiltinname/) | Gets the locale dependent text for built-in Name according to given standard text. |
|[GetStandardBuiltInName](./getstandardbuiltinname/) | Gets the standard text of built-in Name according to given locale dependent text. |
|[GetListSeparator](./getlistseparator/) | Gets the separator for list, parameters of function, ...etc. |
|[GetRowSeparatorOfFormulaArray](./getrowseparatorofformulaarray/) | Gets the separator for rows in array data in formula. |
|[GetColumnSeparatorOfFormulaArray](./getcolumnseparatorofformulaarray/) | Gets the separator for the items in array's row data in formula. |
|[GetStandardHeaderFooterFontStyleName](./getstandardheaderfooterfontstylename/) | Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name. |
|[GetCommentTitleName](./getcommenttitlename/) | Gets the locale dependent comment title name according to comment title type. |
|[Compare](./compare/) | Compares two string values according to certain collation rules. |
