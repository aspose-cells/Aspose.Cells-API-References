---
title: "SettableGlobalizationSettings Class"
linktitle: "SettableGlobalizationSettings"
articleTitle: "SettableGlobalizationSettings"
second_title: "Aspose.Cells for Python via Java"
description: "Implementation of GlobalizationSettings that supports user to set/change pre-defined texts."
type: docs
weight: 5770
url: /python-java/asposecells.api/settableglobalizationsettings/
---

## SettableGlobalizationSettings class

Implementation of GlobalizationSettings that supports user to set/change pre-defined texts.

## Constructors

| Name | Description |
| --- | --- |
| [SettableGlobalizationSettings](#constructor) |  |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [ListSeparator](#listseparator) | char | Gets the separator for list, parameters of function, ...etc. |
| [RowSeparatorOfFormulaArray](#rowseparatorofformulaarray) | char | Gets the separator for rows in array data in formula. |
| [ColumnSeparatorOfFormulaArray](#columnseparatorofformulaarray) | char | Gets the separator for the items in array's row data in formula. |
| [ChartSettings](#chartsettings) | ChartGlobalizationSettings | Gets or sets the globalization settings for Chart. |
| [PivotSettings](#pivotsettings) | PivotGlobalizationSettings | Gets or sets the globalization settings for pivot table. |

## Methods

| Name | Description |
| --- | --- |
| [getTotalName](#gettotalname) | Gets the total name of specific function. |
| [setTotalName](#settotalname) | Sets the total name of specific function. |
| [getGrandTotalName](#getgrandtotalname) | Gets the grand total name of the function. |
| [setGrandTotalName](#setgrandtotalname) | Sets the grand total name of specific function. |
| [getTableRowTypeOfHeaders](#gettablerowtypeofheaders) | Gets the type name of table rows that consists of the table header. Default is "Headers", so in formula "#Headers" repre |
| [setTableRowTypeOfHeaders](#settablerowtypeofheaders) | Sets the type name of table rows that consists of the table header. |
| [getTableRowTypeOfData](#gettablerowtypeofdata) | Gets the type name of table rows that consists of data region of referenced table. Default is "Data", so in formula "#Da |
| [setTableRowTypeOfData](#settablerowtypeofdata) | Sets the type name of table rows that consists of data region of referenced table. |
| [getTableRowTypeOfAll](#gettablerowtypeofall) | Gets the type name of table rows that consists of all rows in referenced table. |
| [setTableRowTypeOfAll](#settablerowtypeofall) | Sets the type name of table rows that consists of all rows in referenced table. |
| [getTableRowTypeOfTotals](#gettablerowtypeoftotals) | Gets the type name of table rows that consists of the total row of referenced table. |
| [setTableRowTypeOfTotals](#settablerowtypeoftotals) | Sets the type name of table rows that consists of the total row of referenced table. |
| [getTableRowTypeOfCurrent](#gettablerowtypeofcurrent) | Gets the type name of table rows that consists of the current row in referenced table. |
| [setTableRowTypeOfCurrent](#settablerowtypeofcurrent) | Sets the type name of table rows that consists of the current row in referenced table. |
| [getErrorValueString](#geterrorvaluestring) | Gets the display string value for cell's error value |
| [getBooleanValueString](#getbooleanvaluestring) | Gets the display string value for cell's boolean value |
| [setBooleanValueString](#setbooleanvaluestring) | Sets the display string value for cell's boolean value |
| [getLocalFunctionName](#getlocalfunctionname) | Gets the locale dependent function name according to given standard function name. |
| [setLocalFunctionName](#setlocalfunctionname) | Sets the locale dependent function name corresponding to given standard function name. |
| [getStandardFunctionName](#getstandardfunctionname) | Gets the standard function name according to given locale dependent function name. |
| [setStandardFunctionName](#setstandardfunctionname) | Sets the locale dependent function name according to given standard function name. |
| [getLocalBuiltInName](#getlocalbuiltinname) | Gets the locale dependent text for built-in Name according to given standard text. |
| [setLocalBuiltInName](#setlocalbuiltinname) | Sets the locale dependent text for the built-in name with given standard name text. |
| [getStandardBuiltInName](#getstandardbuiltinname) | Gets the standard text of built-in Name according to given locale dependent text. |
| [setStandardBuiltInName](#setstandardbuiltinname) | Sets the locale dependent function name according to given standard function name. |
| [setListSeparator](#setlistseparator) | Sets the separator for list, parameters of function, ...etc. |
| [setRowSeparatorOfFormulaArray](#setrowseparatorofformulaarray) | Sets the separator for rows in array data in formula. |
| [setColumnSeparatorOfFormulaArray](#setcolumnseparatorofformulaarray) | Sets the separator for the items in array's row data in formula. |
| [getStandardHeaderFooterFontStyleName](#getstandardheaderfooterfontstylename) | Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name |
| [setStandardHeaderFooterFontStyleName](#setstandardheaderfooterfontstylename) | Sets the locale dependent function name according to given standard function name. |
| [getCommentTitleName](#getcommenttitlename) | Gets the locale dependent comment title name according to comment title type. |
| [setCommentTitleName](#setcommenttitlename) | Gets the locale dependent comment title name according to comment title type. |
| [getPivotTotalName](#getpivottotalname) | Gets the name of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or m |
| [getPivotGrandTotalName](#getpivotgrandtotalname) | Gets the name of "Grand Total" label in the PivotTable.

NOTE: This member is now obsolete. Instead, please use PivotGlo |
| [getMultipleItemsName](#getmultipleitemsname) | Gets the name of "(Multiple Items)" label in the PivotTable.

NOTE: This member is now obsolete. Instead, please use Piv |
| [getAllName](#getallname) | Gets the name of "(All)" label in the PivotTable.

NOTE: This member is now obsolete. Instead, please use GlobalizationS |
| [getProtectionNameOfPivotTable](#getprotectionnameofpivottable) | Gets the protection name in the PivotTable.

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSe |
| [getColumnLabelsOfPivotTable](#getcolumnlabelsofpivottable) | Gets the name of "Column Labels" label in the PivotTable.

NOTE: This member is now obsolete. Instead, please use PivotG |
| [getRowLabelsNameOfPivotTable](#getrowlabelsnameofpivottable) | Gets the name of "Row Labels" label in the PivotTable.

NOTE: This member is now obsolete. Instead, please use PivotGlob |
| [getEmptyDataName](#getemptydataname) | Gets the name of "(blank)" label in the PivotTable.

NOTE: This member is now obsolete. Instead, please use PivotGlobali |
| [getDataFieldHeaderNameOfPivotTable](#getdatafieldheadernameofpivottable) | Gets the the name of the value area field header in the PivotTable.

NOTE: This member is now obsolete. Instead, please  |
| [getSubTotalName](#getsubtotalname) | Gets the name of PivotFieldSubtotalType type in the PivotTable.

NOTE: This member is now obsolete. Instead, please use  |
| [getDefaultSheetName](#getdefaultsheetname) | Gets the default sheet name for adding worksheet automatically. Default is "Sheet".

The automatically added(such as by  |
| [compare](#compare) | Compares two string values according to certain collation rules. |
| [getCollationKey](#getcollationkey) | Transforms the string into a comparable object according to certain collation rules. |

### SettableGlobalizationSettings() {#constructor}

### SettableGlobalizationSettings.ListSeparator property {#listseparator}

Gets the separator for list, parameters of function, ...etc.

**Type:** char

### SettableGlobalizationSettings.RowSeparatorOfFormulaArray property {#rowseparatorofformulaarray}

Gets the separator for rows in array data in formula.

**Type:** char

### SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray property {#columnseparatorofformulaarray}

Gets the separator for the items in array's row data in formula.

**Type:** char

### SettableGlobalizationSettings.ChartSettings property {#chartsettings}

Gets or sets the globalization settings for Chart.

**Type:** ChartGlobalizationSettings

### SettableGlobalizationSettings.PivotSettings property {#pivotsettings}

Gets or sets the globalization settings for pivot table.

**Type:** PivotGlobalizationSettings

### getTotalName(functionType) {#gettotalname}

Gets the total name of specific function.

| Parameter | Type | Description |
| --- | --- | --- |
| functionType | int | A ConsolidationFunction value. The function type. |

**Returns:** The total name of the function.

### setTotalName(functionType, name) {#settotalname}

Sets the total name of specific function.

| Parameter | Type | Description |
| --- | --- | --- |
| functionType | int | A ConsolidationFunction value. The function type. |
| name | String | The total name of the function. |

### getGrandTotalName(functionType) {#getgrandtotalname}

Gets the grand total name of the function.

| Parameter | Type | Description |
| --- | --- | --- |
| functionType | int | A ConsolidationFunction value. The function type. |

**Returns:** The grand total name of the function.

### setGrandTotalName(functionType, name) {#setgrandtotalname}

Sets the grand total name of specific function.

| Parameter | Type | Description |
| --- | --- | --- |
| functionType | int | A ConsolidationFunction value. The function type. |
| name | String | The grand total name of the function. |

### getTableRowTypeOfHeaders() {#gettablerowtypeofheaders}

Gets the type name of table rows that consists of the table header. Default is "Headers", so in formula "#Headers" represents the table header.

**Returns:** the type name of table rows

### setTableRowTypeOfHeaders(name) {#settablerowtypeofheaders}

Sets the type name of table rows that consists of the table header.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | the type name of table rows |

### getTableRowTypeOfData() {#gettablerowtypeofdata}

Gets the type name of table rows that consists of data region of referenced table. Default is "Data", so in formula "#Data" represents the data region of the table.

**Returns:** the type name of table rows

### setTableRowTypeOfData(name) {#settablerowtypeofdata}

Sets the type name of table rows that consists of data region of referenced table.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | the type name of table rows |

### getTableRowTypeOfAll() {#gettablerowtypeofall}

Gets the type name of table rows that consists of all rows in referenced table.

**Returns:** the type name of table rows

### setTableRowTypeOfAll(name) {#settablerowtypeofall}

Sets the type name of table rows that consists of all rows in referenced table.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | the type name of table rows |

### getTableRowTypeOfTotals() {#gettablerowtypeoftotals}

Gets the type name of table rows that consists of the total row of referenced table.

**Returns:** the type name of table rows

### setTableRowTypeOfTotals(name) {#settablerowtypeoftotals}

Sets the type name of table rows that consists of the total row of referenced table.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | the type name of table rows |

### getTableRowTypeOfCurrent() {#gettablerowtypeofcurrent}

Gets the type name of table rows that consists of the current row in referenced table.

**Returns:** the type name of table rows

### setTableRowTypeOfCurrent(name) {#settablerowtypeofcurrent}

Sets the type name of table rows that consists of the current row in referenced table.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | the type name of table rows |

### getErrorValueString(err) {#geterrorvaluestring}

Gets the display string value for cell's error value

| Parameter | Type | Description |
| --- | --- | --- |
| err | String | error values such as #VALUE!,#NAME? |

**Returns:** By default returns the error value itself

### getBooleanValueString(bv) {#getbooleanvaluestring}

Gets the display string value for cell's boolean value

| Parameter | Type | Description |
| --- | --- | --- |
| bv | boolean | boolean value |

**Returns:** By default returns "TRUE" for true value and "FALSE" for false value.

### setBooleanValueString(bv, name) {#setbooleanvaluestring}

Sets the display string value for cell's boolean value

| Parameter | Type | Description |
| --- | --- | --- |
| bv | boolean | boolean value |
| name | String | string value of the boolean value |

### getLocalFunctionName(standardName) {#getlocalfunctionname}

Gets the locale dependent function name according to given standard function name.

| Parameter | Type | Description |
| --- | --- | --- |
| standardName | String | Standard(en-US locale) function name. |

**Returns:** Locale dependent function name. The locale was specified by the Workbook for which this settings is used.

### setLocalFunctionName(standardName, localName, bidirectional) {#setlocalfunctionname}

Sets the locale dependent function name corresponding to given standard function name.

| Parameter | Type | Description |
| --- | --- | --- |
| standardName | String | Standard(en-US locale) function name. |
| localName | String | Locale dependent function name |
| bidirectional | boolean | Whether map the local function name to standard function name automatically. If true, the local name will be mapped to standard name automatically so user does not need to call setStandardFunctionName(java.lang.String, java.lang.String, boolean) again for the same standard and local names pair |

### getStandardFunctionName(localName) {#getstandardfunctionname}

Gets the standard function name according to given locale dependent function name.

| Parameter | Type | Description |
| --- | --- | --- |
| localName | String | Locale dependent function name. The locale was specified by the Workbook for which this settings is used. |

**Returns:** Standard(en-US locale) function name.

### setStandardFunctionName(localName, standardName, bidirectional) {#setstandardfunctionname}

Sets the locale dependent function name according to given standard function name.

| Parameter | Type | Description |
| --- | --- | --- |
| localName | String | Locale dependent function name |
| standardName | String | Standard(en-US locale) function name. |
| bidirectional | boolean | Whether map the standard function name to local function name automatically. If true, the standar name will be mapped to local name automatically so user does not need to call setLocalFunctionName(java.lang.String, java.lang.String, boolean) again for the same standard and local names pair |

### getLocalBuiltInName(standardName) {#getlocalbuiltinname}

Gets the locale dependent text for built-in Name according to given standard text.

| Parameter | Type | Description |
| --- | --- | --- |
| standardName | String | Standard(en-US locale) text of built-in Name. |

**Returns:** Locale dependent text. The locale was specified by the Workbook for which this settings is used.

### setLocalBuiltInName(standardName, localName, bidirectional) {#setlocalbuiltinname}

Sets the locale dependent text for the built-in name with given standard name text.

| Parameter | Type | Description |
| --- | --- | --- |
| standardName | String | Standard(en-US locale) name text of built-in name. |
| localName | String | Locale dependent name text |
| bidirectional | boolean | Whether map the local name text to standard name text automatically. If true, the local name text will be mapped to standard name text automatically so user does not need to call setStandardBuiltInName(java.lang.String, java.lang.String, boolean) again for the same standard and local names pair |

### getStandardBuiltInName(localName) {#getstandardbuiltinname}

Gets the standard text of built-in Name according to given locale dependent text.

| Parameter | Type | Description |
| --- | --- | --- |
| localName | String | Locale dependent text of built-in Name. The locale was specified by the Workbook for which this settings is used. |

**Returns:** Standard(en-US locale) text.

### setStandardBuiltInName(localName, standardName, bidirectional) {#setstandardbuiltinname}

Sets the locale dependent function name according to given standard function name.

| Parameter | Type | Description |
| --- | --- | --- |
| localName | String | Locale dependent function name |
| standardName | String | Standard(en-US locale) function name. |
| bidirectional | boolean | Whether map the standard name text to local name text automatically. If true, the standar name text will be mapped to local name text automatically so user does not need to call setLocalBuiltInName(java.lang.String, java.lang.String, boolean) again for the same standard and local names pair |

### setListSeparator(c) {#setlistseparator}

Sets the separator for list, parameters of function, ...etc.

| Parameter | Type | Description |
| --- | --- | --- |
| c | char | the specified separator |

### setRowSeparatorOfFormulaArray(c) {#setrowseparatorofformulaarray}

Sets the separator for rows in array data in formula.

| Parameter | Type | Description |
| --- | --- | --- |
| c | char | the specified separator |

### setColumnSeparatorOfFormulaArray(c) {#setcolumnseparatorofformulaarray}

Sets the separator for the items in array's row data in formula.

| Parameter | Type | Description |
| --- | --- | --- |
| c | char | the specified separator |

### getStandardHeaderFooterFontStyleName(localfontStyleName) {#getstandardheaderfooterfontstylename}

Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name.

| Parameter | Type | Description |
| --- | --- | --- |
| localfontStyleName | String | Locale font style name for Header/Footer. |

**Returns:** Standard English font style name(Regular, Bold, Italic)

### setStandardHeaderFooterFontStyleName(localfontStyleName, standardName) {#setstandardheaderfooterfontstylename}

Sets the locale dependent function name according to given standard function name.

| Parameter | Type | Description |
| --- | --- | --- |
| localfontStyleName | String | Locale font style name for Header/Footer. |
| standardName | String | Standard(en-US locale) function name. |

### getCommentTitleName(type) {#getcommenttitlename}

Gets the locale dependent comment title name according to comment title type.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A CommentTitleType value. type of comment title |

**Returns:** locale dependent comment title name

### setCommentTitleName(type, name) {#setcommenttitlename}

Gets the locale dependent comment title name according to comment title type.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A CommentTitleType value. type of comment title |
| name | String | locale dependent comment title name |

### getPivotTotalName() {#getpivottotalname}

Gets the name of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area.

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:** The name of "Total" label

### getPivotGrandTotalName() {#getpivotgrandtotalname}

Gets the name of "Grand Total" label in the PivotTable.

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:** The name of "Grand Total" label

### getMultipleItemsName() {#getmultipleitemsname}

Gets the name of "(Multiple Items)" label in the PivotTable.

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:** The name of "(Multiple Items)" label

### getAllName() {#getallname}

Gets the name of "(All)" label in the PivotTable.

NOTE: This member is now obsolete. Instead, please use GlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:** The name of "(All)" label

### getProtectionNameOfPivotTable() {#getprotectionnameofpivottable}

Gets the protection name in the PivotTable.

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetTextOfProtectedName(string) method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:** The protection name of PivotTable

### getColumnLabelsOfPivotTable() {#getcolumnlabelsofpivottable}

Gets the name of "Column Labels" label in the PivotTable.

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:** The name of column labels

### getRowLabelsNameOfPivotTable() {#getrowlabelsnameofpivottable}

Gets the name of "Row Labels" label in the PivotTable.

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:** The name of row labels

### getEmptyDataName() {#getemptydataname}

Gets the name of "(blank)" label in the PivotTable.

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:** The name of empty data

### getDataFieldHeaderNameOfPivotTable() {#getdatafieldheadernameofpivottable}

Gets the the name of the value area field header in the PivotTable.

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:** The name of data field header name

### getSubTotalName(subTotalType) {#getsubtotalname}

Gets the name of PivotFieldSubtotalType type in the PivotTable.

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| subTotalType | int | A PivotFieldSubtotalType value. The PivotFieldSubtotalType type |

**Returns:** The name of PivotFieldSubtotalType type

### getDefaultSheetName() {#getdefaultsheetname}

Gets the default sheet name for adding worksheet automatically. Default is "Sheet".

The automatically added(such as by WorksheetCollection.add() ) sheet's name will be the specified name plus sequence number. For example, for Germany user maybe wants the sheet name to be "Tabellenblatt2" instead of "Sheet2". Then user may implement this method to return "Tabellenblatt".

**Returns:** the default sheet name for adding worksheet automatically

### compare(v1, v2, ignoreCase) {#compare}

Compares two string values according to certain collation rules.

| Parameter | Type | Description |
| --- | --- | --- |
| v1 | String | the first string |
| v2 | String | the second string |
| ignoreCase | boolean | whether ignore case when comparing values |

**Returns:** Integer that indicates the lexical relationship between the two comparands

### getCollationKey(v, ignoreCase) {#getcollationkey}

Transforms the string into a comparable object according to certain collation rules.

| Parameter | Type | Description |
| --- | --- | --- |
| v | String | String value needs to be compared with others. |
| ignoreCase | boolean | whether ignore case when comparing values |

**Returns:** Object can be used to compare or sort string values
