---
title: "GlobalizationSettings Class"
linktitle: "GlobalizationSettings"
articleTitle: "GlobalizationSettings"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents the globalization settings."
type: docs
weight: 2650
url: /php/aspose.cells/globalizationsettings/
---

## GlobalizationSettings class

Represents the globalization settings.

## Constructors

| Name | Description |
| --- | --- |
| [GlobalizationSettings](#constructor) |  |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [ChartSettings](#chartsettings) | ChartGlobalizationSettings | Gets or sets the globalization settings for Chart. |
| [PivotSettings](#pivotsettings) | PivotGlobalizationSettings | Gets or sets the globalization settings for pivot table. |
| [ListSeparator](#listseparator) | char | Gets the separator for list, parameters of function, ...etc. |
| [RowSeparatorOfFormulaArray](#rowseparatorofformulaarray) | char | Gets the separator for rows in array data in formula. |
| [ColumnSeparatorOfFormulaArray](#columnseparatorofformulaarray) | char | Gets the separator for the items in array's row data in formula. |

## Methods

| Name | Description |
| --- | --- |
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
| [getTotalName](#gettotalname) | Gets the total name of the function. |
| [getGrandTotalName](#getgrandtotalname) | Gets the grand total name of the function. |
| [getDefaultSheetName](#getdefaultsheetname) | Gets the default sheet name for adding worksheet automatically. Default is "Sheet".

The automatically added(such as by  |
| [getTableRowTypeOfHeaders](#gettablerowtypeofheaders) | Gets the type name of table rows that consists of the table header. Default is "Headers", so in formula "#Headers" repre |
| [getTableRowTypeOfData](#gettablerowtypeofdata) | Gets the type name of table rows that consists of data region of referenced table. Default is "Data", so in formula "#Da |
| [getTableRowTypeOfAll](#gettablerowtypeofall) | Gets the type name of table rows that consists of all rows in referenced table. Default is "All", so in formula "#All" r |
| [getTableRowTypeOfTotals](#gettablerowtypeoftotals) | Gets the type name of table rows that consists of the total row of referenced table. Default is "Totals", so in formula  |
| [getTableRowTypeOfCurrent](#gettablerowtypeofcurrent) | Gets the type name of table rows that consists of the current row in referenced table. Default is "This Row", so in form |
| [getErrorValueString](#geterrorvaluestring) | Gets the display string value for cell's error value |
| [getBooleanValueString](#getbooleanvaluestring) | Gets the display string value for cell's boolean value |
| [getLocalFunctionName](#getlocalfunctionname) | Gets the locale dependent function name according to given standard function name. |
| [getStandardFunctionName](#getstandardfunctionname) | Gets the standard function name according to given locale dependent function name. |
| [getLocalBuiltInName](#getlocalbuiltinname) | Gets the locale dependent text for built-in Name according to given standard text. |
| [getStandardBuiltInName](#getstandardbuiltinname) | Gets the standard text of built-in Name according to given locale dependent text. |
| [getStandardHeaderFooterFontStyleName](#getstandardheaderfooterfontstylename) | Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name |
| [getCommentTitleName](#getcommenttitlename) | Gets the locale dependent comment title name according to comment title type. |
| [compare](#compare) | Compares two string values according to certain collation rules. |
| [getCollationKey](#getcollationkey) | Transforms the string into a comparable object according to certain collation rules. |

### GlobalizationSettings() {#constructor}

### GlobalizationSettings.ChartSettings property {#chartsettings}

Gets or sets the globalization settings for Chart.

**Type:** ChartGlobalizationSettings

### GlobalizationSettings.PivotSettings property {#pivotsettings}

Gets or sets the globalization settings for pivot table.

**Type:** PivotGlobalizationSettings

### GlobalizationSettings.ListSeparator property {#listseparator}

Gets the separator for list, parameters of function, ...etc.

**Type:** char

### GlobalizationSettings.RowSeparatorOfFormulaArray property {#rowseparatorofformulaarray}

Gets the separator for rows in array data in formula.

**Type:** char

### GlobalizationSettings.ColumnSeparatorOfFormulaArray property {#columnseparatorofformulaarray}

Gets the separator for the items in array's row data in formula.

**Type:** char

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
| subTotalType | Number | A PivotFieldSubtotalType value. The PivotFieldSubtotalType type |

**Returns:** The name of PivotFieldSubtotalType type

### getTotalName(functionType) {#gettotalname}

Gets the total name of the function.

| Parameter | Type | Description |
| --- | --- | --- |
| functionType | Number | A ConsolidationFunction value. The function type. |

**Returns:** The total name of the function.

### getGrandTotalName(functionType) {#getgrandtotalname}

Gets the grand total name of the function.

| Parameter | Type | Description |
| --- | --- | --- |
| functionType | Number | A ConsolidationFunction value. The function type. |

**Returns:** The grand total name of the function.

### getDefaultSheetName() {#getdefaultsheetname}

Gets the default sheet name for adding worksheet automatically. Default is "Sheet".

The automatically added(such as by WorksheetCollection.add() ) sheet's name will be the specified name plus sequence number. For example, for Germany user maybe wants the sheet name to be "Tabellenblatt2" instead of "Sheet2". Then user may implement this method to return "Tabellenblatt".

**Returns:** the default sheet name for adding worksheet automatically

### getTableRowTypeOfHeaders() {#gettablerowtypeofheaders}

Gets the type name of table rows that consists of the table header. Default is "Headers", so in formula "#Headers" represents the table header.

**Returns:** the type name of table rows

### getTableRowTypeOfData() {#gettablerowtypeofdata}

Gets the type name of table rows that consists of data region of referenced table. Default is "Data", so in formula "#Data" represents the data region of the table.

**Returns:** the type name of table rows

### getTableRowTypeOfAll() {#gettablerowtypeofall}

Gets the type name of table rows that consists of all rows in referenced table. Default is "All", so in formula "#All" represents all rows in referenced table.

**Returns:** the type name of table rows

### getTableRowTypeOfTotals() {#gettablerowtypeoftotals}

Gets the type name of table rows that consists of the total row of referenced table. Default is "Totals", so in formula "#Totals" represents the total row of referenced table.

**Returns:** the type name of table rows

### getTableRowTypeOfCurrent() {#gettablerowtypeofcurrent}

Gets the type name of table rows that consists of the current row in referenced table. Default is "This Row", so in formula "#This Row" represents the current row in referenced table.

**Returns:** the type name of table rows

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

### getLocalFunctionName(standardName) {#getlocalfunctionname}

Gets the locale dependent function name according to given standard function name.

| Parameter | Type | Description |
| --- | --- | --- |
| standardName | String | Standard(en-US locale) function name. |

**Returns:** Locale dependent function name. The locale was specified by the Workbook for which this settings is used.

### getStandardFunctionName(localName) {#getstandardfunctionname}

Gets the standard function name according to given locale dependent function name.

| Parameter | Type | Description |
| --- | --- | --- |
| localName | String | Locale dependent function name. The locale was specified by the Workbook for which this settings is used. |

**Returns:** Standard(en-US locale) function name.

### getLocalBuiltInName(standardName) {#getlocalbuiltinname}

Gets the locale dependent text for built-in Name according to given standard text.

| Parameter | Type | Description |
| --- | --- | --- |
| standardName | String | Standard(en-US locale) text of built-in Name. |

**Returns:** Locale dependent text. The locale was specified by the Workbook for which this settings is used.

### getStandardBuiltInName(localName) {#getstandardbuiltinname}

Gets the standard text of built-in Name according to given locale dependent text.

| Parameter | Type | Description |
| --- | --- | --- |
| localName | String | Locale dependent text of built-in Name. The locale was specified by the Workbook for which this settings is used. |

**Returns:** Standard(en-US locale) text.

### getStandardHeaderFooterFontStyleName(localfontStyleName) {#getstandardheaderfooterfontstylename}

Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name.

| Parameter | Type | Description |
| --- | --- | --- |
| localfontStyleName | String | Locale font style name for Header/Footer. |

**Returns:** Standard English font style name(Regular, Bold, Italic)

### getCommentTitleName(type) {#getcommenttitlename}

Gets the locale dependent comment title name according to comment title type.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | A CommentTitleType value. |

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
