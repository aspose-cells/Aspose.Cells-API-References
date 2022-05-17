---
title: GlobalizationSettings
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 3610
url: /net/aspose.cells/globalizationsettings/
---
## GlobalizationSettings class

Represents the globalization settings.

```csharp
public class GlobalizationSettings : AbstractGlobalizationSettings
```

## Constructors

| Name | Description |
| --- | --- |
| [GlobalizationSettings](globalizationsettings)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [ChartSettings](chartsettings) { get; set; } | Gets or sets the Chart of this[`ChartGlobalizationSettings`](../../aspose.cells.charts/chartglobalizationsettings) |
| virtual [ColumnSeparatorOfFormulaArray](columnseparatorofformulaarray) { get; } | Gets the separator for the items in array's row data in formula. |
| virtual [ListSeparator](listseparator) { get; } | Gets the separator for list, parameters of function, ...etc. |
| virtual [RowSeparatorOfFormulaArray](rowseparatorofformulaarray) { get; } | Gets the separator for rows in array data in formula. |

## Methods

| Name | Description |
| --- | --- |
| virtual [GetAllName](getallname)() | Gets the name of "(All)" label in the PivotTable. |
| virtual [GetBooleanValueString](getbooleanvaluestring)(bool) | Gets the display string value for cell's boolean value |
| virtual [GetColumnLabelsOfPivotTable](getcolumnlabelsofpivottable)() | Gets the name of "Column Labels" label in the PivotTable. |
| virtual [GetCommentTitleName](getcommenttitlename)(CommentTitleType) | Gets the locale dependent comment title name according to comment title type. |
| virtual [GetEmptyDataName](getemptydataname)() | Gets the name of "(blank)" label in the PivotTable. |
| virtual [GetErrorValueString](geterrorvaluestring)(string) | Gets the display string value for cell's error value |
| virtual [GetGrandTotalName](getgrandtotalname)(ConsolidationFunction) | Gets the grand total name of the function. |
| virtual [GetLocalBuiltInName](getlocalbuiltinname)(string) | Gets the locale dependent text for built-in Name according to given standard text. |
| virtual [GetLocalFunctionName](getlocalfunctionname)(string) | Gets the locale dependent function name according to given standard function name. |
| virtual [GetMultipleItemsName](getmultipleitemsname)() | Gets the name of "(Multiple Items)" label in the PivotTable. |
| virtual [GetOtherName](getothername)() | Gets the name of "Other" labels for Pie charts. |
| virtual [GetPivotGrandTotalName](getpivotgrandtotalname)() | Gets the name of "Grand Total" label in the PivotTable. |
| virtual [GetPivotTotalName](getpivottotalname)() | Gets the name of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area. |
| virtual [GetProtectionNameOfPivotTable](getprotectionnameofpivottable)() | Gets the protection name in the PivotTable. |
| virtual [GetRowLabelsNameOfPivotTable](getrowlabelsnameofpivottable)() | Gets the name of "Row Labels" label in the PivotTable. |
| virtual [GetStandardBuiltInName](getstandardbuiltinname)(string) | Gets the standard text of built-in Name according to given locale dependent text. |
| virtual [GetStandardFunctionName](getstandardfunctionname)(string) | Gets the standard function name according to given locale dependent function name. |
| virtual [GetStandardHeaderFooterFontStyleName](getstandardheaderfooterfontstylename)(string) | Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name. |
| virtual [GetSubTotalName](getsubtotalname)(PivotFieldSubtotalType) | Gets the name of [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype) type in the PivotTable. |
| virtual [GetTableRowTypeOfAll](gettablerowtypeofall)() | Gets the type name of table rows that consists of all rows in referenced table. Default is "All", so in formula "#All" represents all rows in referenced table. |
| virtual [GetTableRowTypeOfCurrent](gettablerowtypeofcurrent)() | Gets the type name of table rows that consists of the current row in referenced table. Default is "This Row", so in formula "#This Row" represents the current row in referenced table. |
| virtual [GetTableRowTypeOfData](gettablerowtypeofdata)() | Gets the type name of table rows that consists of data region of referenced table. Default is "Data", so in formula "#Data" represents the data region of the table. |
| virtual [GetTableRowTypeOfHeaders](gettablerowtypeofheaders)() | Gets the type name of table rows that consists of the table header. Default is "Headers", so in formula "#Headers" represents the table header. |
| virtual [GetTableRowTypeOfTotals](gettablerowtypeoftotals)() | Gets the type name of table rows that consists of the total row of referenced table. Default is "Totals", so in formula "#Totals" represents the total row of referenced table. |
| virtual [GetTotalName](gettotalname)(ConsolidationFunction) | Gets the total name of the function. |

### See Also

* class [AbstractGlobalizationSettings](../abstractglobalizationsettings)
* namespace [Aspose.Cells](../../aspose.cells)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
