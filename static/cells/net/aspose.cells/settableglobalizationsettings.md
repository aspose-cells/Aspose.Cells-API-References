##Class SettableGlobalizationSettings
Aspose.Cells.SettableGlobalizationSettings class. Implementation of GlobalizationSettings that supports user to set/change predefined texts
## SettableGlobalizationSettings class
Implementation of GlobalizationSettings that supports user to set/change pre-defined texts.
```csharp
public class SettableGlobalizationSettings : GlobalizationSettings
```
## Constructors
| Name | Description |
| --- | --- |
| [SettableGlobalizationSettings](settableglobalizationsettings/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings/) { get; set; } | Gets or sets the globalization settings for Chart.(Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| override [ColumnSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/columnseparatorofformulaarray/) { get; } | Gets the separator for the items in array's row data in formula. |
| override [ListSeparator](../../aspose.cells/settableglobalizationsettings/listseparator/) { get; } | Gets the separator for list, parameters of function, ...etc. |
| [PivotSettings](../../aspose.cells/globalizationsettings/pivotsettings/) { get; set; } | Gets or sets the globalization settings for pivot table.(Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| override [RowSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/rowseparatorofformulaarray/) { get; } | Gets the separator for rows in array data in formula. |
## Methods
| Name | Description |
| --- | --- |
| virtual [Compare](../../aspose.cells/globalizationsettings/compare/)(string, string, bool) | Compares two string values according to certain collation rules.(Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname/)() | (**Obsolete.**) Gets the name of "(All)" label in the PivotTable.(Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetBooleanValueString](../../aspose.cells/settableglobalizationsettings/getbooleanvaluestring/)(bool) | Gets the display string value for cell's boolean value |
| virtual [GetCollationKey](../../aspose.cells/globalizationsettings/getcollationkey/)(string, bool) | Transforms the string into a comparable object according to certain collation rules.(Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/)() | (**Obsolete.**) Gets the name of "Column Labels" label in the PivotTable.(Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetCommentTitleName](../../aspose.cells/settableglobalizationsettings/getcommenttitlename/)(CommentTitleType) | Gets the locale dependent comment title name according to comment title type. |
| virtual [GetDataFieldHeaderNameOfPivotTable](../../aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/)() | (**Obsolete.**) Gets the the name of the value area field header in the PivotTable.(Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetDefaultSheetName](../../aspose.cells/globalizationsettings/getdefaultsheetname/)() | Gets the default sheet name for adding worksheet automatically. Default is "Sheet".(Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname/)() | (**Obsolete.**) Gets the name of "(blank)" label in the PivotTable.(Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetErrorValueString](../../aspose.cells/settableglobalizationsettings/geterrorvaluestring/)(string) | Gets the display string value for cell's error value |
| override [GetGrandTotalName](../../aspose.cells/settableglobalizationsettings/getgrandtotalname/)(ConsolidationFunction) | Gets the grand total name of the function. |
| override [GetLocalBuiltInName](../../aspose.cells/settableglobalizationsettings/getlocalbuiltinname/)(string) | Gets the locale dependent text for built-in Name according to given standard text. |
| override [GetLocalFunctionName](../../aspose.cells/settableglobalizationsettings/getlocalfunctionname/)(string) | Gets the locale dependent function name according to given standard function name. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname/)() | (**Obsolete.**) Gets the name of "(Multiple Items)" label in the PivotTable.(Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname/)() | (**Obsolete.**) Gets the name of "Grand Total" label in the PivotTable.(Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname/)() | (**Obsolete.**) Gets the name of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area.(Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable/)() | (**Obsolete.**) Gets the protection name in the PivotTable.(Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/)() | (**Obsolete.**) Gets the name of "Row Labels" label in the PivotTable.(Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetStandardBuiltInName](../../aspose.cells/settableglobalizationsettings/getstandardbuiltinname/)(string) | Gets the standard text of built-in Name according to given locale dependent text. |
| override [GetStandardFunctionName](../../aspose.cells/settableglobalizationsettings/getstandardfunctionname/)(string) | Gets the standard function name according to given locale dependent function name. |
| override [GetStandardHeaderFooterFontStyleName](../../aspose.cells/settableglobalizationsettings/getstandardheaderfooterfontstylename/)(string) | Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname/)(PivotFieldSubtotalType) | (**Obsolete.**) Gets the name of [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) type in the PivotTable.(Inherited from [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetTableRowTypeOfAll](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofall/)() | Gets the type name of table rows that consists of all rows in referenced table. |
| override [GetTableRowTypeOfCurrent](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofcurrent/)() | Gets the type name of table rows that consists of the current row in referenced table. |
| override [GetTableRowTypeOfData](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofdata/)() | Gets the type name of table rows that consists of data region of referenced table. Default is "Data", so in formula "#Data" represents the data region of the table. |
| override [GetTableRowTypeOfHeaders](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofheaders/)() | Gets the type name of table rows that consists of the table header. Default is "Headers", so in formula "#Headers" represents the table header. |
| override [GetTableRowTypeOfTotals](../../aspose.cells/settableglobalizationsettings/gettablerowtypeoftotals/)() | Gets the type name of table rows that consists of the total row of referenced table. |
| override [GetTotalName](../../aspose.cells/settableglobalizationsettings/gettotalname/)(ConsolidationFunction) | Gets the total name of specific function. |
| [SetBooleanValueString](../../aspose.cells/settableglobalizationsettings/setbooleanvaluestring/)(bool, string) | Sets the display string value for cell's boolean value |
| [SetColumnSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/setcolumnseparatorofformulaarray/)(char) | Sets the separator for the items in array's row data in formula. |
| [SetCommentTitleName](../../aspose.cells/settableglobalizationsettings/setcommenttitlename/)(CommentTitleType, string) | Gets the locale dependent comment title name according to comment title type. |
| [SetGrandTotalName](../../aspose.cells/settableglobalizationsettings/setgrandtotalname/)(ConsolidationFunction, string) | Sets the grand total name of specific function. |
| [SetListSeparator](../../aspose.cells/settableglobalizationsettings/setlistseparator/)(char) | Sets the separator for list, parameters of function, ...etc. |
| [SetLocalBuiltInName](../../aspose.cells/settableglobalizationsettings/setlocalbuiltinname/)(string, string, bool) | Sets the locale dependent text for the built-in name with given standard name text. |
| [SetLocalFunctionName](../../aspose.cells/settableglobalizationsettings/setlocalfunctionname/)(string, string, bool) | Sets the locale dependent function name corresponding to given standard function name. |
| [SetRowSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/setrowseparatorofformulaarray/)(char) | Sets the separator for rows in array data in formula. |
| [SetStandardBuiltInName](../../aspose.cells/settableglobalizationsettings/setstandardbuiltinname/)(string, string, bool) | Sets the locale dependent function name according to given standard function name. |
| [SetStandardFunctionName](../../aspose.cells/settableglobalizationsettings/setstandardfunctionname/)(string, string, bool) | Sets the locale dependent function name according to given standard function name. |
| [SetStandardHeaderFooterFontStyleName](../../aspose.cells/settableglobalizationsettings/setstandardheaderfooterfontstylename/)(string, string) | Sets the locale dependent function name according to given standard function name. |
| [SetTableRowTypeOfAll](../../aspose.cells/settableglobalizationsettings/settablerowtypeofall/)(string) | Sets the type name of table rows that consists of all rows in referenced table. |
| [SetTableRowTypeOfCurrent](../../aspose.cells/settableglobalizationsettings/settablerowtypeofcurrent/)(string) | Sets the type name of table rows that consists of the current row in referenced table. |
| [SetTableRowTypeOfData](../../aspose.cells/settableglobalizationsettings/settablerowtypeofdata/)(string) | Sets the type name of table rows that consists of data region of referenced table. |
| [SetTableRowTypeOfHeaders](../../aspose.cells/settableglobalizationsettings/settablerowtypeofheaders/)(string) | Sets the type name of table rows that consists of the table header. |
| [SetTableRowTypeOfTotals](../../aspose.cells/settableglobalizationsettings/settablerowtypeoftotals/)(string) | Sets the type name of table rows that consists of the total row of referenced table. |
| [SetTotalName](../../aspose.cells/settableglobalizationsettings/settotalname/)(ConsolidationFunction, string) | Sets the total name of specific function. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
public class CellsClassSettableGlobalizationSettingsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of SettableGlobalizationSettings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
// Set custom list separator
settings.SetListSeparator(';');
// Set custom boolean value strings
settings.SetBooleanValueString(true, "TRUE_CUSTOM");
settings.SetBooleanValueString(false, "FALSE_CUSTOM");
// Set custom function names
settings.SetLocalFunctionName("SUM", "SUMME", true);
settings.SetLocalFunctionName("AVERAGE", "MITTELWERT", true);
// Set custom table row type names
settings.SetTableRowTypeOfHeaders("HEADERS_CUSTOM");
settings.SetTableRowTypeOfData("DATA_CUSTOM");
settings.SetTableRowTypeOfTotals("TOTALS_CUSTOM");
// Set custom comment title names
settings.SetCommentTitleName(CommentTitleType.Comment, "COMMENT_CUSTOM");
// Removed the Author line since CommentTitleType doesn't have that enum value
// If you need to set author-related settings, you would need to use ThreadedCommentAuthor instead
// Apply the globalization settings to the workbook
workbook.Settings.GlobalizationSettings = settings;
// Demonstrate usage in formulas
worksheet.Cells["A1"].Formula = "=TRUE()";
worksheet.Cells["A2"].Formula = "=FALSE()";
worksheet.Cells["A3"].Formula = "=SUM(1,2,3)";
worksheet.Cells["A4"].Formula = "=AVERAGE(1,2,3)";
// Save the workbook
workbook.Save("SettableGlobalizationSettingsDemo.xlsx");
}
}
}
```
### See Also
* class [GlobalizationSettings](../globalizationsettings/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
