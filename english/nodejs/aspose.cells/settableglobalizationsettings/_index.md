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
| [compare(v1, v2, ignoreCase)](#compare) | Compares two string values according to certain collation rules. |
| [getAllName()](#getallname) | Gets the name of "(All)" label in the PivotTable. NOTE: This member is now obsolete. Instead, please use GlobalizationSe |
| [getBooleanValueString(bv)](#getbooleanvaluestring) | Gets the display string value for cell's boolean value |
| [getChartSettings()](#getchartsettings) | Gets or sets the globalization settings for Chart. |
| [getCollationKey(v, ignoreCase)](#getcollationkey) | Transforms the string into a comparable object according to certain collation rules. |
| [getColumnLabelsOfPivotTable()](#getcolumnlabelsofpivottable) | Gets the name of "Column Labels" label in the PivotTable. NOTE: This member is now obsolete. Instead, please use PivotGl |
| [getColumnSeparatorOfFormulaArray()](#getcolumnseparatorofformulaarray) | Gets the separator for the items in array's row data in formula. |
| [getCommentTitleName(type)](#getcommenttitlename) | Gets the locale dependent comment title name according to comment title type. |
| [getDataFieldHeaderNameOfPivotTable()](#getdatafieldheadernameofpivottable) | Gets the the name of the value area field header in the PivotTable. NOTE: This member is now obsolete. Instead, please u |
| [getDefaultSheetName()](#getdefaultsheetname) | Gets the default sheet name for adding worksheet automatically. Default is "Sheet". The automatically added(such as by W |
| [getEmptyDataName()](#getemptydataname) | Gets the name of "(blank)" label in the PivotTable. NOTE: This member is now obsolete. Instead, please use PivotGlobaliz |
| [getErrorValueString(err)](#geterrorvaluestring) | Gets the display string value for cell's error value |
| [getGrandTotalName(functionType)](#getgrandtotalname) | Gets the grand total name of the function. |
| [getListSeparator()](#getlistseparator) | Gets the separator for list, parameters of function, ...etc. |
| [getLocalBuiltInName(standardName)](#getlocalbuiltinname) | Gets the locale dependent text for built-in Name according to given standard text. |
| [getLocalFunctionName(standardName)](#getlocalfunctionname) | Gets the locale dependent function name according to given standard function name. |
| [getMultipleItemsName()](#getmultipleitemsname) | Gets the name of "(Multiple Items)" label in the PivotTable. NOTE: This member is now obsolete. Instead, please use Pivo |
| [getPivotGrandTotalName()](#getpivotgrandtotalname) | Gets the name of "Grand Total" label in the PivotTable. NOTE: This member is now obsolete. Instead, please use PivotGlob |
| [getPivotSettings()](#getpivotsettings) | Gets or sets the globalization settings for pivot table. |
| [getPivotTotalName()](#getpivottotalname) | Gets the name of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or m |
| [getProtectionNameOfPivotTable()](#getprotectionnameofpivottable) | Gets the protection name in the PivotTable. NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSet |
| [getRowLabelsNameOfPivotTable()](#getrowlabelsnameofpivottable) | Gets the name of "Row Labels" label in the PivotTable. NOTE: This member is now obsolete. Instead, please use PivotGloba |
| [getRowSeparatorOfFormulaArray()](#getrowseparatorofformulaarray) | Gets the separator for rows in array data in formula. |
| [getStandardBuiltInName(localName)](#getstandardbuiltinname) | Gets the standard text of built-in Name according to given locale dependent text. |
| [getStandardFunctionName(localName)](#getstandardfunctionname) | Gets the standard function name according to given locale dependent function name. |
| [getStandardHeaderFooterFontStyleName(localfontStyleName)](#getstandardheaderfooterfontstylename) | Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name |
| [getSubTotalName(subTotalType)](#getsubtotalname) | Gets the name of PivotFieldSubtotalType type in the PivotTable. NOTE: This member is now obsolete. Instead, please use P |
| [getTableRowTypeOfAll()](#gettablerowtypeofall) | Gets the type name of table rows that consists of all rows in referenced table. |
| [getTableRowTypeOfCurrent()](#gettablerowtypeofcurrent) | Gets the type name of table rows that consists of the current row in referenced table. |
| [getTableRowTypeOfData()](#gettablerowtypeofdata) | Gets the type name of table rows that consists of data region of referenced table. Default is "Data", so in formula "#Da |
| [getTableRowTypeOfHeaders()](#gettablerowtypeofheaders) | Gets the type name of table rows that consists of the table header. Default is "Headers", so in formula "#Headers" repre |
| [getTableRowTypeOfTotals()](#gettablerowtypeoftotals) | Gets the type name of table rows that consists of the total row of referenced table. |
| [getTotalName(functionType)](#gettotalname) | Gets the total name of specific function. |
| [setBooleanValueString(bv, name)](#setbooleanvaluestring) | Sets the display string value for cell's boolean value |
| [setChartSettings()](#setchartsettings) | Gets or sets the globalization settings for Chart. |
| [setColumnSeparatorOfFormulaArray(c)](#setcolumnseparatorofformulaarray) | Sets the separator for the items in array's row data in formula. |
| [setCommentTitleName(type, name)](#setcommenttitlename) | Gets the locale dependent comment title name according to comment title type. |
| [setGrandTotalName(functionType, name)](#setgrandtotalname) | Sets the grand total name of specific function. |
| [setListSeparator(c)](#setlistseparator) | Sets the separator for list, parameters of function, ...etc. |
| [setLocalBuiltInName(standardName, localName, bidirectional)](#setlocalbuiltinname) | Sets the locale dependent text for the built-in name with given standard name text. |
| [setLocalFunctionName(standardName, localName, bidirectional)](#setlocalfunctionname) | Sets the locale dependent function name corresponding to given standard function name. |
| [setPivotSettings()](#setpivotsettings) | Gets or sets the globalization settings for pivot table. |
| [setRowSeparatorOfFormulaArray(c)](#setrowseparatorofformulaarray) | Sets the separator for rows in array data in formula. |
| [setStandardBuiltInName(localName, standardName, bidirectional)](#setstandardbuiltinname) | Sets the locale dependent function name according to given standard function name. |
| [setStandardFunctionName(localName, standardName, bidirectional)](#setstandardfunctionname) | Sets the locale dependent function name according to given standard function name. |
| [setStandardHeaderFooterFontStyleName(localfontStyleName, standardName)](#setstandardheaderfooterfontstylename) | Sets the locale dependent function name according to given standard function name. |
| [setTableRowTypeOfAll(name)](#settablerowtypeofall) | Sets the type name of table rows that consists of all rows in referenced table. |
| [setTableRowTypeOfCurrent(name)](#settablerowtypeofcurrent) | Sets the type name of table rows that consists of the current row in referenced table. |
| [setTableRowTypeOfData(name)](#settablerowtypeofdata) | Sets the type name of table rows that consists of data region of referenced table. |
| [setTableRowTypeOfHeaders(name)](#settablerowtypeofheaders) | Sets the type name of table rows that consists of the table header. |
| [setTableRowTypeOfTotals(name)](#settablerowtypeoftotals) | Sets the type name of table rows that consists of the total row of referenced table. |
| [setTotalName(functionType, name)](#settotalname) | Sets the total name of specific function. |

### compare(v1, v2, ignoreCase) {#compare}

Compares two string values according to certain collation rules.

| Parameter | Type | Description |
| --- | --- | --- |
| v1 | String | the first string |
| v2 | String | the second string |
| ignoreCase | boolean | whether ignore case when comparing values |

**Returns:** Number — `Number` Integer that indicates the lexical relationship between the two comparands

### getAllName() {#getallname}

Gets the name of "(All)" label in the PivotTable. NOTE: This member is now obsolete. Instead, please use GlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.@return {String} The name of "(All)" label

### getBooleanValueString(bv) {#getbooleanvaluestring}

Gets the display string value for cell's boolean value

| Parameter | Type | Description |
| --- | --- | --- |
| bv | boolean | boolean value |

**Returns:** String — `String` By default returns "TRUE" for true value and "FALSE" for false value.

### getChartSettings() {#getchartsettings}

Gets or sets the globalization settings for Chart.

### getCollationKey(v, ignoreCase) {#getcollationkey}

Transforms the string into a comparable object according to certain collation rules.

| Parameter | Type | Description |
| --- | --- | --- |
| v | String | String value needs to be compared with others. |
| ignoreCase | boolean | whether ignore case when comparing values |

**Returns:** IComparable — `IComparable` Object can be used to compare or sort string values

### getColumnLabelsOfPivotTable() {#getcolumnlabelsofpivottable}

Gets the name of "Column Labels" label in the PivotTable. NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.@return {String} The name of column labels

### getColumnSeparatorOfFormulaArray() {#getcolumnseparatorofformulaarray}

Gets the separator for the items in array's row data in formula.

### getCommentTitleName(type) {#getcommenttitlename}

Gets the locale dependent comment title name according to comment title type.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | CommentTitleType |

**Returns:** String — `String` locale dependent comment title name

### getDataFieldHeaderNameOfPivotTable() {#getdatafieldheadernameofpivottable}

Gets the the name of the value area field header in the PivotTable. NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.@return {String} The name of data field header name

### getDefaultSheetName() {#getdefaultsheetname}

Gets the default sheet name for adding worksheet automatically. Default is "Sheet". The automatically added(such as by WorksheetCollection.add()) sheet's name will be the specified name plus sequence number. For example, for Germany user maybe wants the sheet name to be "Tabellenblatt2" instead of "Sheet2". Then user may implement this method to return "Tabellenblatt".@return {String} the default sheet name for adding worksheet automatically

### getEmptyDataName() {#getemptydataname}

Gets the name of "(blank)" label in the PivotTable. NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.@return {String} The name of empty data

### getErrorValueString(err) {#geterrorvaluestring}

Gets the display string value for cell's error value

| Parameter | Type | Description |
| --- | --- | --- |
| err | String | error values such as #VALUE!,#NAME? |

**Returns:** String — `String` By default returns the error value itself

### getGrandTotalName(functionType) {#getgrandtotalname}

Gets the grand total name of the function.

| Parameter | Type | Description |
| --- | --- | --- |
| functionType | Number | ConsolidationFunction |

**Returns:** String — `String` The grand total name of the function.

### getListSeparator() {#getlistseparator}

Gets the separator for list, parameters of function, ...etc.

### getLocalBuiltInName(standardName) {#getlocalbuiltinname}

Gets the locale dependent text for built-in Name according to given standard text.

| Parameter | Type | Description |
| --- | --- | --- |
| standardName | String | Standard(en-US locale) text of built-in Name. |

**Returns:** String — `String` Locale dependent text. The locale was specified by the Workbook for which this settings is used.

### getLocalFunctionName(standardName) {#getlocalfunctionname}

Gets the locale dependent function name according to given standard function name.

| Parameter | Type | Description |
| --- | --- | --- |
| standardName | String | Standard(en-US locale) function name. |

**Returns:** String — `String` Locale dependent function name. The locale was specified by the Workbook for which this settings is used.

### getMultipleItemsName() {#getmultipleitemsname}

Gets the name of "(Multiple Items)" label in the PivotTable. NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.@return {String} The name of "(Multiple Items)" label

### getPivotGrandTotalName() {#getpivotgrandtotalname}

Gets the name of "Grand Total" label in the PivotTable. NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.@return {String} The name of "Grand Total" label

### getPivotSettings() {#getpivotsettings}

Gets or sets the globalization settings for pivot table.

### getPivotTotalName() {#getpivottotalname}

Gets the name of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area. NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.@return {String} The name of "Total" label

### getProtectionNameOfPivotTable() {#getprotectionnameofpivottable}

Gets the protection name in the PivotTable. NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetTextOfProtectedName(string) method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.@return {String} The protection name of PivotTable

### getRowLabelsNameOfPivotTable() {#getrowlabelsnameofpivottable}

Gets the name of "Row Labels" label in the PivotTable. NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.@return {String} The name of row labels

### getRowSeparatorOfFormulaArray() {#getrowseparatorofformulaarray}

Gets the separator for rows in array data in formula.

### getStandardBuiltInName(localName) {#getstandardbuiltinname}

Gets the standard text of built-in Name according to given locale dependent text.

| Parameter | Type | Description |
| --- | --- | --- |
| localName | String | Locale dependent text of built-in Name. The locale was specified by the Workbook for which this settings is used. |

**Returns:** String — `String` Standard(en-US locale) text.

### getStandardFunctionName(localName) {#getstandardfunctionname}

Gets the standard function name according to given locale dependent function name.

| Parameter | Type | Description |
| --- | --- | --- |
| localName | String | Locale dependent function name. The locale was specified by the Workbook for which this settings is used. |

**Returns:** String — `String` Standard(en-US locale) function name.

### getStandardHeaderFooterFontStyleName(localfontStyleName) {#getstandardheaderfooterfontstylename}

Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name.

| Parameter | Type | Description |
| --- | --- | --- |
| localfontStyleName | String | Locale font style name for Header/Footer. |

**Returns:** String — `String` Standard English font style name(Regular, Bold, Italic)

### getSubTotalName(subTotalType) {#getsubtotalname}

Gets the name of PivotFieldSubtotalType type in the PivotTable. NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| subTotalType | Number | PivotFieldSubtotalType |

**Returns:** String — `String` The name of PivotFieldSubtotalType type

### getTableRowTypeOfAll() {#gettablerowtypeofall}

Gets the type name of table rows that consists of all rows in referenced table.

**Returns:** String — `String` the type name of table rows

### getTableRowTypeOfCurrent() {#gettablerowtypeofcurrent}

Gets the type name of table rows that consists of the current row in referenced table.

**Returns:** String — `String` the type name of table rows

### getTableRowTypeOfData() {#gettablerowtypeofdata}

Gets the type name of table rows that consists of data region of referenced table. Default is "Data", so in formula "#Data" represents the data region of the table.

**Returns:** String — `String` the type name of table rows

### getTableRowTypeOfHeaders() {#gettablerowtypeofheaders}

Gets the type name of table rows that consists of the table header. Default is "Headers", so in formula "#Headers" represents the table header.

**Returns:** String — `String` the type name of table rows

### getTableRowTypeOfTotals() {#gettablerowtypeoftotals}

Gets the type name of table rows that consists of the total row of referenced table.

**Returns:** String — `String` the type name of table rows

### getTotalName(functionType) {#gettotalname}

Gets the total name of specific function.

| Parameter | Type | Description |
| --- | --- | --- |
| functionType | Number | ConsolidationFunction |

**Returns:** String — `String` The total name of the function.

### setBooleanValueString(bv, name) {#setbooleanvaluestring}

Sets the display string value for cell's boolean value

| Parameter | Type | Description |
| --- | --- | --- |
| bv | boolean | boolean value |
| name | String | string value of the boolean value |

### setChartSettings() {#setchartsettings}

Gets or sets the globalization settings for Chart.

### setColumnSeparatorOfFormulaArray(c) {#setcolumnseparatorofformulaarray}

Sets the separator for the items in array's row data in formula.

| Parameter | Type | Description |
| --- | --- | --- |
| c | char | the specified separator |

### setCommentTitleName(type, name) {#setcommenttitlename}

Gets the locale dependent comment title name according to comment title type.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | CommentTitleType |
| name | String | locale dependent comment title name |

### setGrandTotalName(functionType, name) {#setgrandtotalname}

Sets the grand total name of specific function.

| Parameter | Type | Description |
| --- | --- | --- |
| functionType | Number | ConsolidationFunction |
| name | String | The grand total name of the function. |

### setListSeparator(c) {#setlistseparator}

Sets the separator for list, parameters of function, ...etc.

| Parameter | Type | Description |
| --- | --- | --- |
| c | char | the specified separator |

### setLocalBuiltInName(standardName, localName, bidirectional) {#setlocalbuiltinname}

Sets the locale dependent text for the built-in name with given standard name text.

| Parameter | Type | Description |
| --- | --- | --- |
| standardName | String | Standard(en-US locale) name text of built-in name. |
| localName | String | Locale dependent name text |
| bidirectional | boolean | Whether map the local name text to standard name text automatically. If true, the local name text will be mapped to standard name text automatically so user does not need to call |

### setLocalFunctionName(standardName, localName, bidirectional) {#setlocalfunctionname}

Sets the locale dependent function name corresponding to given standard function name.

| Parameter | Type | Description |
| --- | --- | --- |
| standardName | String | Standard(en-US locale) function name. |
| localName | String | Locale dependent function name |
| bidirectional | boolean | Whether map the local function name to standard function name automatically. If true, the local name will be mapped to standard name automatically so user does not need to call |

### setPivotSettings() {#setpivotsettings}

Gets or sets the globalization settings for pivot table.

### setRowSeparatorOfFormulaArray(c) {#setrowseparatorofformulaarray}

Sets the separator for rows in array data in formula.

| Parameter | Type | Description |
| --- | --- | --- |
| c | char | the specified separator |

### setStandardBuiltInName(localName, standardName, bidirectional) {#setstandardbuiltinname}

Sets the locale dependent function name according to given standard function name.

| Parameter | Type | Description |
| --- | --- | --- |
| localName | String | Locale dependent function name |
| standardName | String | Standard(en-US locale) function name. |
| bidirectional | boolean | Whether map the standard name text to local name text automatically. If true, the standar name text will be mapped to local name text automatically so user does not need to call |

### setStandardFunctionName(localName, standardName, bidirectional) {#setstandardfunctionname}

Sets the locale dependent function name according to given standard function name.

| Parameter | Type | Description |
| --- | --- | --- |
| localName | String | Locale dependent function name |
| standardName | String | Standard(en-US locale) function name. |
| bidirectional | boolean | Whether map the standard function name to local function name automatically. If true, the standar name will be mapped to local name automatically so user does not need to call |

### setStandardHeaderFooterFontStyleName(localfontStyleName, standardName) {#setstandardheaderfooterfontstylename}

Sets the locale dependent function name according to given standard function name.

| Parameter | Type | Description |
| --- | --- | --- |
| localfontStyleName | String | Locale font style name for Header/Footer. |
| standardName | String | Standard(en-US locale) function name. |

### setTableRowTypeOfAll(name) {#settablerowtypeofall}

Sets the type name of table rows that consists of all rows in referenced table.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | the type name of table rows |

### setTableRowTypeOfCurrent(name) {#settablerowtypeofcurrent}

Sets the type name of table rows that consists of the current row in referenced table.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | the type name of table rows |

### setTableRowTypeOfData(name) {#settablerowtypeofdata}

Sets the type name of table rows that consists of data region of referenced table.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | the type name of table rows |

### setTableRowTypeOfHeaders(name) {#settablerowtypeofheaders}

Sets the type name of table rows that consists of the table header.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | the type name of table rows |

### setTableRowTypeOfTotals(name) {#settablerowtypeoftotals}

Sets the type name of table rows that consists of the total row of referenced table.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | the type name of table rows |

### setTotalName(functionType, name) {#settotalname}

Sets the total name of specific function.

| Parameter | Type | Description |
| --- | --- | --- |
| functionType | Number | ConsolidationFunction |
| name | String | The total name of the function. |
