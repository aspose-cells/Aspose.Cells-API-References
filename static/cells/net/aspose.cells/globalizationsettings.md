##Class GlobalizationSettings
Aspose.Cells.GlobalizationSettings class. Represents the globalization settings
## GlobalizationSettings class
Represents the globalization settings.
```csharp
public class GlobalizationSettings
```
## Constructors
| Name | Description |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings/) { get; set; } | Gets or sets the globalization settings for Chart. |
| virtual [ColumnSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/columnseparatorofformulaarray/) { get; } | Gets the separator for the items in array's row data in formula. |
| virtual [ListSeparator](../../aspose.cells/globalizationsettings/listseparator/) { get; } | Gets the separator for list, parameters of function, ...etc. |
| [PivotSettings](../../aspose.cells/globalizationsettings/pivotsettings/) { get; set; } | Gets or sets the globalization settings for pivot table. |
| virtual [RowSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/rowseparatorofformulaarray/) { get; } | Gets the separator for rows in array data in formula. |
## Methods
| Name | Description |
| --- | --- |
| virtual [Compare](../../aspose.cells/globalizationsettings/compare/)(string, string, bool) | Compares two string values according to certain collation rules. |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname/)() | (**Obsolete.**) Gets the name of "(All)" label in the PivotTable. |
| virtual [GetBooleanValueString](../../aspose.cells/globalizationsettings/getbooleanvaluestring/)(bool) | Gets the display string value for cell's boolean value |
| virtual [GetCollationKey](../../aspose.cells/globalizationsettings/getcollationkey/)(string, bool) | Transforms the string into a comparable object according to certain collation rules. |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/)() | (**Obsolete.**) Gets the name of "Column Labels" label in the PivotTable. |
| virtual [GetCommentTitleName](../../aspose.cells/globalizationsettings/getcommenttitlename/)(CommentTitleType) | Gets the locale dependent comment title name according to comment title type. |
| virtual [GetDataFieldHeaderNameOfPivotTable](../../aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/)() | (**Obsolete.**) Gets the the name of the value area field header in the PivotTable. |
| virtual [GetDefaultSheetName](../../aspose.cells/globalizationsettings/getdefaultsheetname/)() | Gets the default sheet name for adding worksheet automatically. Default is "Sheet". |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname/)() | (**Obsolete.**) Gets the name of "(blank)" label in the PivotTable. |
| virtual [GetErrorValueString](../../aspose.cells/globalizationsettings/geterrorvaluestring/)(string) | Gets the display string value for cell's error value |
| virtual [GetGrandTotalName](../../aspose.cells/globalizationsettings/getgrandtotalname/)(ConsolidationFunction) | Gets the grand total name of the function. |
| virtual [GetLocalBuiltInName](../../aspose.cells/globalizationsettings/getlocalbuiltinname/)(string) | Gets the locale dependent text for built-in Name according to given standard text. |
| virtual [GetLocalFunctionName](../../aspose.cells/globalizationsettings/getlocalfunctionname/)(string) | Gets the locale dependent function name according to given standard function name. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname/)() | (**Obsolete.**) Gets the name of "(Multiple Items)" label in the PivotTable. |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname/)() | (**Obsolete.**) Gets the name of "Grand Total" label in the PivotTable. |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname/)() | (**Obsolete.**) Gets the name of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area. |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable/)() | (**Obsolete.**) Gets the protection name in the PivotTable. |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/)() | (**Obsolete.**) Gets the name of "Row Labels" label in the PivotTable. |
| virtual [GetStandardBuiltInName](../../aspose.cells/globalizationsettings/getstandardbuiltinname/)(string) | Gets the standard text of built-in Name according to given locale dependent text. |
| virtual [GetStandardFunctionName](../../aspose.cells/globalizationsettings/getstandardfunctionname/)(string) | Gets the standard function name according to given locale dependent function name. |
| virtual [GetStandardHeaderFooterFontStyleName](../../aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename/)(string) | Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname/)(PivotFieldSubtotalType) | (**Obsolete.**) Gets the name of [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) type in the PivotTable. |
| virtual [GetTableRowTypeOfAll](../../aspose.cells/globalizationsettings/gettablerowtypeofall/)() | Gets the type name of table rows that consists of all rows in referenced table. Default is "All", so in formula "#All" represents all rows in referenced table. |
| virtual [GetTableRowTypeOfCurrent](../../aspose.cells/globalizationsettings/gettablerowtypeofcurrent/)() | Gets the type name of table rows that consists of the current row in referenced table. Default is "This Row", so in formula "#This Row" represents the current row in referenced table. |
| virtual [GetTableRowTypeOfData](../../aspose.cells/globalizationsettings/gettablerowtypeofdata/)() | Gets the type name of table rows that consists of data region of referenced table. Default is "Data", so in formula "#Data" represents the data region of the table. |
| virtual [GetTableRowTypeOfHeaders](../../aspose.cells/globalizationsettings/gettablerowtypeofheaders/)() | Gets the type name of table rows that consists of the table header. Default is "Headers", so in formula "#Headers" represents the table header. |
| virtual [GetTableRowTypeOfTotals](../../aspose.cells/globalizationsettings/gettablerowtypeoftotals/)() | Gets the type name of table rows that consists of the total row of referenced table. Default is "Totals", so in formula "#Totals" represents the total row of referenced table. |
| virtual [GetTotalName](../../aspose.cells/globalizationsettings/gettotalname/)(ConsolidationFunction) | Gets the total name of the function. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassGlobalizationSettingsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add sample data
cells["A1"].PutValue("Region");
cells["B1"].PutValue("Sales");
cells["A2"].PutValue("North");
cells["B2"].PutValue(1000);
cells["A3"].PutValue("South");
cells["B3"].PutValue(2000);
cells["A4"].PutValue("East");
cells["B4"].PutValue(3000);
cells["A5"].PutValue("West");
cells["B5"].PutValue(4000);
// Create and apply globalization settings
GlobalizationSettings settings = new CustomGlobalizationSettings();
workbook.Settings.GlobalizationSettings = settings;
// Apply subtotal with custom globalization
CellArea area = CellArea.CreateCellArea(0, 0, 5, 1);
cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 0 }, true, false, true);
// Save the workbook
workbook.Save("output.xlsx");
}
}
public class CustomGlobalizationSettings : GlobalizationSettings
{
public override string GetTotalName(ConsolidationFunction functionType)
{
// Customize the total name based on function type
switch (functionType)
{
case ConsolidationFunction.Sum:
return "Custom Sum";
case ConsolidationFunction.Count:
return "Custom Count";
default:
return base.GetTotalName(functionType);
}
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
