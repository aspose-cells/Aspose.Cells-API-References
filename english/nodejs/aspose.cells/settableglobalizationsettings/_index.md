---
title: "SettableGlobalizationSettings"
linktitle: "SettableGlobalizationSettings"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Implementation of GlobalizationSettings that supports user to set/change pre-defined texts."
type: docs
weight: 3520
url: /nodejs/aspose.cells/settableglobalizationsettings/
---

## SettableGlobalizationSettings class

Implementation of GlobalizationSettings that supports user to set/change pre-defined texts.

```js
new SettableGlobalizationSettings()
```

## Methods

| Name | Description |
| --- | --- |
| [compare(v1, v2, ignoreCase)](./compare/) | Compares two string values according to certain collation rules. |
| [getAllName()](./getallname/) | Gets the name of "(All)" label in the PivotTable. NOTE: This member is now obsolete. Instead, please use GlobalizationSe |
| [getBooleanValueString(bv)](./getbooleanvaluestring/) | Gets the display string value for cell's boolean value |
| [getChartSettings()](./getchartsettings/) | Gets or sets the globalization settings for Chart. |
| [getCollationKey(v, ignoreCase)](./getcollationkey/) | Transforms the string into a comparable object according to certain collation rules. |
| [getColumnLabelsOfPivotTable()](./getcolumnlabelsofpivottable/) | Gets the name of "Column Labels" label in the PivotTable. NOTE: This member is now obsolete. Instead, please use PivotGl |
| [getColumnSeparatorOfFormulaArray()](./getcolumnseparatorofformulaarray/) | Gets the separator for the items in array's row data in formula. |
| [getCommentTitleName(type)](./getcommenttitlename/) | Gets the locale dependent comment title name according to comment title type. |
| [getDataFieldHeaderNameOfPivotTable()](./getdatafieldheadernameofpivottable/) | Gets the the name of the value area field header in the PivotTable. NOTE: This member is now obsolete. Instead, please u |
| [getDefaultSheetName()](./getdefaultsheetname/) | Gets the default sheet name for adding worksheet automatically. Default is "Sheet". The automatically added(such as by W |
| [getEmptyDataName()](./getemptydataname/) | Gets the name of "(blank)" label in the PivotTable. NOTE: This member is now obsolete. Instead, please use PivotGlobaliz |
| [getErrorValueString(err)](./geterrorvaluestring/) | Gets the display string value for cell's error value |
| [getGrandTotalName(functionType)](./getgrandtotalname/) | Gets the grand total name of the function. |
| [getListSeparator()](./getlistseparator/) | Gets the separator for list, parameters of function, ...etc. |
| [getLocalBuiltInName(standardName)](./getlocalbuiltinname/) | Gets the locale dependent text for built-in Name according to given standard text. |
| [getLocalFunctionName(standardName)](./getlocalfunctionname/) | Gets the locale dependent function name according to given standard function name. |
| [getMultipleItemsName()](./getmultipleitemsname/) | Gets the name of "(Multiple Items)" label in the PivotTable. NOTE: This member is now obsolete. Instead, please use Pivo |
| [getPivotGrandTotalName()](./getpivotgrandtotalname/) | Gets the name of "Grand Total" label in the PivotTable. NOTE: This member is now obsolete. Instead, please use PivotGlob |
| [getPivotSettings()](./getpivotsettings/) | Gets or sets the globalization settings for pivot table. |
| [getPivotTotalName()](./getpivottotalname/) | Gets the name of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or m |
| [getProtectionNameOfPivotTable()](./getprotectionnameofpivottable/) | Gets the protection name in the PivotTable. NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSet |
| [getRowLabelsNameOfPivotTable()](./getrowlabelsnameofpivottable/) | Gets the name of "Row Labels" label in the PivotTable. NOTE: This member is now obsolete. Instead, please use PivotGloba |
| [getRowSeparatorOfFormulaArray()](./getrowseparatorofformulaarray/) | Gets the separator for rows in array data in formula. |
| [getStandardBuiltInName(localName)](./getstandardbuiltinname/) | Gets the standard text of built-in Name according to given locale dependent text. |
| [getStandardFunctionName(localName)](./getstandardfunctionname/) | Gets the standard function name according to given locale dependent function name. |
| [getStandardHeaderFooterFontStyleName(localfontStyleName)](./getstandardheaderfooterfontstylename/) | Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name |
| [getSubTotalName(subTotalType)](./getsubtotalname/) | Gets the name of PivotFieldSubtotalType type in the PivotTable. NOTE: This member is now obsolete. Instead, please use P |
| [getTableRowTypeOfAll()](./gettablerowtypeofall/) | Gets the type name of table rows that consists of all rows in referenced table. |
| [getTableRowTypeOfCurrent()](./gettablerowtypeofcurrent/) | Gets the type name of table rows that consists of the current row in referenced table. |
| [getTableRowTypeOfData()](./gettablerowtypeofdata/) | Gets the type name of table rows that consists of data region of referenced table. Default is "Data", so in formula "#Da |
| [getTableRowTypeOfHeaders()](./gettablerowtypeofheaders/) | Gets the type name of table rows that consists of the table header. Default is "Headers", so in formula "#Headers" repre |
| [getTableRowTypeOfTotals()](./gettablerowtypeoftotals/) | Gets the type name of table rows that consists of the total row of referenced table. |
| [getTotalName(functionType)](./gettotalname/) | Gets the total name of specific function. |
| [setBooleanValueString(bv, name)](./setbooleanvaluestring/) | Sets the display string value for cell's boolean value |
| [setChartSettings()](./setchartsettings/) | Gets or sets the globalization settings for Chart. |
| [setColumnSeparatorOfFormulaArray(c)](./setcolumnseparatorofformulaarray/) | Sets the separator for the items in array's row data in formula. |
| [setCommentTitleName(type, name)](./setcommenttitlename/) | Gets the locale dependent comment title name according to comment title type. |
| [setGrandTotalName(functionType, name)](./setgrandtotalname/) | Sets the grand total name of specific function. |
| [setListSeparator(c)](./setlistseparator/) | Sets the separator for list, parameters of function, ...etc. |
| [setLocalBuiltInName(standardName, localName, bidirectional)](./setlocalbuiltinname/) | Sets the locale dependent text for the built-in name with given standard name text. |
| [setLocalFunctionName(standardName, localName, bidirectional)](./setlocalfunctionname/) | Sets the locale dependent function name corresponding to given standard function name. |
| [setPivotSettings()](./setpivotsettings/) | Gets or sets the globalization settings for pivot table. |
| [setRowSeparatorOfFormulaArray(c)](./setrowseparatorofformulaarray/) | Sets the separator for rows in array data in formula. |
| [setStandardBuiltInName(localName, standardName, bidirectional)](./setstandardbuiltinname/) | Sets the locale dependent function name according to given standard function name. |
| [setStandardFunctionName(localName, standardName, bidirectional)](./setstandardfunctionname/) | Sets the locale dependent function name according to given standard function name. |
| [setStandardHeaderFooterFontStyleName(localfontStyleName, standardName)](./setstandardheaderfooterfontstylename/) | Sets the locale dependent function name according to given standard function name. |
| [setTableRowTypeOfAll(name)](./settablerowtypeofall/) | Sets the type name of table rows that consists of all rows in referenced table. |
| [setTableRowTypeOfCurrent(name)](./settablerowtypeofcurrent/) | Sets the type name of table rows that consists of the current row in referenced table. |
| [setTableRowTypeOfData(name)](./settablerowtypeofdata/) | Sets the type name of table rows that consists of data region of referenced table. |
| [setTableRowTypeOfHeaders(name)](./settablerowtypeofheaders/) | Sets the type name of table rows that consists of the table header. |
| [setTableRowTypeOfTotals(name)](./settablerowtypeoftotals/) | Sets the type name of table rows that consists of the total row of referenced table. |
| [setTotalName(functionType, name)](./settotalname/) | Sets the total name of specific function. |
