---
title: SettableGlobalizationSettings
second_title: Aspose.Cells for Java API Reference
description: Implementation of GlobalizationSettings that supports user to set/change pre-defined texts.
type: docs
url: /java/com.aspose.cells/settableglobalizationsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.GlobalizationSettings](../../com.aspose.cells/globalizationsettings)
```
public class SettableGlobalizationSettings extends GlobalizationSettings
```

Implementation of GlobalizationSettings that supports user to set/change pre-defined texts.
## Constructors

| Constructor | Description |
| --- | --- |
| [SettableGlobalizationSettings()](#SettableGlobalizationSettings--) |  |
## Methods

| Method | Description |
| --- | --- |
| [compare(String v1, String v2, boolean ignoreCase)](#compare-java.lang.String-java.lang.String-boolean-) | Compares two string values according to certain collation rules. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllName()](#getAllName--) | Gets the name of the "(All)" label in the PivotTable. |
| [getBooleanValueString(boolean bv)](#getBooleanValueString-boolean-) | Gets the display string value for cell's boolean value |
| [getChartSettings()](#getChartSettings--) | Gets the globalization settings for Chart. |
| [getClass()](#getClass--) |  |
| [getCollationKey(String v, boolean ignoreCase)](#getCollationKey-java.lang.String-boolean-) | Transforms the string into a comparable object according to certain collation rules. |
| [getColumnLabelsOfPivotTable()](#getColumnLabelsOfPivotTable--) | Gets the name of the "Column Labels" label in the PivotTable. |
| [getColumnSeparatorOfFormulaArray()](#getColumnSeparatorOfFormulaArray--) | Gets the separator for the items in array's row data in formula. |
| [getCommentTitleName(int type)](#getCommentTitleName-int-) | Gets the locale dependent comment title name according to comment title type. |
| [getDataFieldHeaderNameOfPivotTable()](#getDataFieldHeaderNameOfPivotTable--) | Gets the the name of the value area field header in the PivotTable. |
| [getDefaultSheetName()](#getDefaultSheetName--) | Gets the default sheet name for adding worksheet automatically. |
| [getEmptyDataName()](#getEmptyDataName--) | Gets the name of "(blank)" label in the PivotTable. |
| [getErrorValueString(String err)](#getErrorValueString-java.lang.String-) | Gets the display string value for cell's error value |
| [getGrandTotalName(int functionType)](#getGrandTotalName-int-) | Gets the grand total name of the function. |
| [getListSeparator()](#getListSeparator--) | Gets the separator for list, parameters of function, ...etc. |
| [getLocalBuiltInName(String standardName)](#getLocalBuiltInName-java.lang.String-) | Gets the locale dependent text for built-in Name according to given standard text. |
| [getLocalFunctionName(String standardName)](#getLocalFunctionName-java.lang.String-) | Gets the locale dependent function name according to given standard function name. |
| [getMultipleItemsName()](#getMultipleItemsName--) | Gets the name of the "(Multiple Items)" label in the PivotTable. |
| [getPivotGrandTotalName()](#getPivotGrandTotalName--) | Gets the name of the "Grand Total" label in the PivotTable. |
| [getPivotSettings()](#getPivotSettings--) | Gets the globalization settings for the pivot table. |
| [getPivotTotalName()](#getPivotTotalName--) | Gets the name of "Total" label in the PivotTable. |
| [getProtectionNameOfPivotTable()](#getProtectionNameOfPivotTable--) | Gets the protection name in the PivotTable. |
| [getRowLabelsNameOfPivotTable()](#getRowLabelsNameOfPivotTable--) | Gets the name of "Row Labels" label in the PivotTable. |
| [getRowSeparatorOfFormulaArray()](#getRowSeparatorOfFormulaArray--) | Gets the separator for rows in array data in formula. |
| [getStandardBuiltInName(String localName)](#getStandardBuiltInName-java.lang.String-) | Gets the standard text of built-in Name according to given locale dependent text. |
| [getStandardFunctionName(String localName)](#getStandardFunctionName-java.lang.String-) | Gets the standard function name according to given locale dependent function name. |
| [getStandardHeaderFooterFontStyleName(String localfontStyleName)](#getStandardHeaderFooterFontStyleName-java.lang.String-) | Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name. |
| [getSubTotalName(int subTotalType)](#getSubTotalName-int-) | Gets the name of [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) type in the PivotTable. |
| [getTableRowTypeOfAll()](#getTableRowTypeOfAll--) | Gets the type name of table rows that consists of all rows in referenced table. |
| [getTableRowTypeOfCurrent()](#getTableRowTypeOfCurrent--) | Gets the type name of table rows that consists of the current row in referenced table. |
| [getTableRowTypeOfData()](#getTableRowTypeOfData--) | Gets the type name of table rows that consists of data region of referenced table. |
| [getTableRowTypeOfHeaders()](#getTableRowTypeOfHeaders--) | Gets the type name of table rows that consists of the table header. |
| [getTableRowTypeOfTotals()](#getTableRowTypeOfTotals--) | Gets the type name of table rows that consists of the total row of referenced table. |
| [getTotalName(int functionType)](#getTotalName-int-) | Gets the total name of specific function. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBooleanValueString(boolean bv, String name)](#setBooleanValueString-boolean-java.lang.String-) | Sets the display string value for cell's boolean value |
| [setChartSettings(ChartGlobalizationSettings value)](#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-) | Sets the globalization settings for Chart. |
| [setColumnSeparatorOfFormulaArray(char c)](#setColumnSeparatorOfFormulaArray-char-) | Sets the separator for the items in array's row data in formula. |
| [setCommentTitleName(int type, String name)](#setCommentTitleName-int-java.lang.String-) | Gets the locale dependent comment title name according to comment title type. |
| [setGrandTotalName(int functionType, String name)](#setGrandTotalName-int-java.lang.String-) | Sets the grand total name of specific function. |
| [setListSeparator(char c)](#setListSeparator-char-) | Sets the separator for list, parameters of function, ...etc. |
| [setLocalBuiltInName(String standardName, String localName, boolean bidirectional)](#setLocalBuiltInName-java.lang.String-java.lang.String-boolean-) | Sets the locale dependent text for the built-in name with given standard name text. |
| [setLocalFunctionName(String standardName, String localName, boolean bidirectional)](#setLocalFunctionName-java.lang.String-java.lang.String-boolean-) | Sets the locale dependent function name corresponding to given standard function name. |
| [setPivotSettings(PivotGlobalizationSettings value)](#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-) | Sets the globalization settings for the pivot table. |
| [setRowSeparatorOfFormulaArray(char c)](#setRowSeparatorOfFormulaArray-char-) | Sets the separator for rows in array data in formula. |
| [setStandardBuiltInName(String localName, String standardName, boolean bidirectional)](#setStandardBuiltInName-java.lang.String-java.lang.String-boolean-) | Sets the locale dependent function name according to given standard function name. |
| [setStandardFunctionName(String localName, String standardName, boolean bidirectional)](#setStandardFunctionName-java.lang.String-java.lang.String-boolean-) | Sets the locale dependent function name according to given standard function name. |
| [setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName)](#setStandardHeaderFooterFontStyleName-java.lang.String-java.lang.String-) | Sets the locale dependent function name according to given standard function name. |
| [setTableRowTypeOfAll(String name)](#setTableRowTypeOfAll-java.lang.String-) | Sets the type name of table rows that consists of all rows in referenced table. |
| [setTableRowTypeOfCurrent(String name)](#setTableRowTypeOfCurrent-java.lang.String-) | Sets the type name of table rows that consists of the current row in referenced table. |
| [setTableRowTypeOfData(String name)](#setTableRowTypeOfData-java.lang.String-) | Sets the type name of table rows that consists of data region of referenced table. |
| [setTableRowTypeOfHeaders(String name)](#setTableRowTypeOfHeaders-java.lang.String-) | Sets the type name of table rows that consists of the table header. |
| [setTableRowTypeOfTotals(String name)](#setTableRowTypeOfTotals-java.lang.String-) | Sets the type name of table rows that consists of the total row of referenced table. |
| [setTotalName(int functionType, String name)](#setTotalName-int-java.lang.String-) | Sets the total name of specific function. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SettableGlobalizationSettings() {#SettableGlobalizationSettings--}
```
public SettableGlobalizationSettings()
```


### compare(String v1, String v2, boolean ignoreCase) {#compare-java.lang.String-java.lang.String-boolean-}
```
public int compare(String v1, String v2, boolean ignoreCase)
```


Compares two string values according to certain collation rules.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| v1 | java.lang.String | the first string |
| v2 | java.lang.String | the second string |
| ignoreCase | boolean | whether ignore case when comparing values |

**Returns:**
int - Integer that indicates the lexical relationship between the two comparands
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAllName() {#getAllName--}
```
public String getAllName()
```


Gets the name of the "(All)" label in the PivotTable.

**Remarks**

NOTE: This member is now obsolete. Instead, please use GlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.lang.String - The name of "(All)" label
### getBooleanValueString(boolean bv) {#getBooleanValueString-boolean-}
```
public String getBooleanValueString(boolean bv)
```


Gets the display string value for cell's boolean value

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| bv | boolean | boolean value |

**Returns:**
java.lang.String - By default returns "TRUE" for true value and "FALSE" for false value.
### getChartSettings() {#getChartSettings--}
```
public ChartGlobalizationSettings getChartSettings()
```


Gets the globalization settings for Chart.

**Returns:**
[ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCollationKey(String v, boolean ignoreCase) {#getCollationKey-java.lang.String-boolean-}
```
public Comparable getCollationKey(String v, boolean ignoreCase)
```


Transforms the string into a comparable object according to certain collation rules.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| v | java.lang.String | String value needs to be compared with others. |
| ignoreCase | boolean | whether ignore case when comparing values |

**Returns:**
java.lang.Comparable - Object can be used to compare or sort string values
### getColumnLabelsOfPivotTable() {#getColumnLabelsOfPivotTable--}
```
public String getColumnLabelsOfPivotTable()
```


Gets the name of the "Column Labels" label in the PivotTable.

**Remarks**

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.lang.String - The name of column labels
### getColumnSeparatorOfFormulaArray() {#getColumnSeparatorOfFormulaArray--}
```
public char getColumnSeparatorOfFormulaArray()
```


Gets the separator for the items in array's row data in formula.

**Returns:**
char
### getCommentTitleName(int type) {#getCommentTitleName-int-}
```
public String getCommentTitleName(int type)
```


Gets the locale dependent comment title name according to comment title type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [CommentTitleType](../../com.aspose.cells/commenttitletype). type of comment title |

**Returns:**
java.lang.String - locale dependent comment title name
### getDataFieldHeaderNameOfPivotTable() {#getDataFieldHeaderNameOfPivotTable--}
```
public String getDataFieldHeaderNameOfPivotTable()
```


Gets the the name of the value area field header in the PivotTable.

**Remarks**

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.lang.String - The name of data field header name
### getDefaultSheetName() {#getDefaultSheetName--}
```
public String getDefaultSheetName()
```


Gets the default sheet name for adding worksheet automatically. Default is "Sheet".

**Remarks**

The automatically added(such as by [WorksheetCollection.add()](../../com.aspose.cells/worksheetcollection\#add--)) sheet's name will be the specified name plus sequence number. For example, for Germany user maybe wants the sheet name to be "Tabellenblatt2" instead of "Sheet2". Then user may implement this method to return "Tabellenblatt".

**Returns:**
java.lang.String - the default sheet name for adding worksheet automatically
### getEmptyDataName() {#getEmptyDataName--}
```
public String getEmptyDataName()
```


Gets the name of "(blank)" label in the PivotTable.

**Remarks**

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.lang.String - The name of empty data
### getErrorValueString(String err) {#getErrorValueString-java.lang.String-}
```
public String getErrorValueString(String err)
```


Gets the display string value for cell's error value

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| err | java.lang.String | error values such as \#VALUE!,\#NAME? |

**Returns:**
java.lang.String - By default returns the error value itself
### getGrandTotalName(int functionType) {#getGrandTotalName-int-}
```
public String getGrandTotalName(int functionType)
```


Gets the grand total name of the function.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). The function type. |

**Returns:**
java.lang.String - The grand total name of the function.
### getListSeparator() {#getListSeparator--}
```
public char getListSeparator()
```


Gets the separator for list, parameters of function, ...etc.

**Returns:**
char
### getLocalBuiltInName(String standardName) {#getLocalBuiltInName-java.lang.String-}
```
public String getLocalBuiltInName(String standardName)
```


Gets the locale dependent text for built-in Name according to given standard text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| standardName | java.lang.String | Standard(en-US locale) text of built-in Name. |

**Returns:**
java.lang.String - Locale dependent text. The locale was specified by the Workbook for which this settings is used.
### getLocalFunctionName(String standardName) {#getLocalFunctionName-java.lang.String-}
```
public String getLocalFunctionName(String standardName)
```


Gets the locale dependent function name according to given standard function name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| standardName | java.lang.String | Standard(en-US locale) function name. |

**Returns:**
java.lang.String - Locale dependent function name. The locale was specified by the Workbook for which this settings is used.
### getMultipleItemsName() {#getMultipleItemsName--}
```
public String getMultipleItemsName()
```


Gets the name of the "(Multiple Items)" label in the PivotTable.

**Remarks**

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.lang.String - The name of "(Multiple Items)" label
### getPivotGrandTotalName() {#getPivotGrandTotalName--}
```
public String getPivotGrandTotalName()
```


Gets the name of the "Grand Total" label in the PivotTable.

**Remarks**

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.lang.String - The name of "Grand Total" label
### getPivotSettings() {#getPivotSettings--}
```
public PivotGlobalizationSettings getPivotSettings()
```


Gets the globalization settings for the pivot table.

**Returns:**
[PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)
### getPivotTotalName() {#getPivotTotalName--}
```
public String getPivotTotalName()
```


Gets the name of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area.

**Remarks**

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.lang.String - The name of "Total" label
### getProtectionNameOfPivotTable() {#getProtectionNameOfPivotTable--}
```
public String getProtectionNameOfPivotTable()
```


Gets the protection name in the PivotTable.

**Remarks**

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetTextOfProtectedName(string) method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.lang.String - The protection name of PivotTable
### getRowLabelsNameOfPivotTable() {#getRowLabelsNameOfPivotTable--}
```
public String getRowLabelsNameOfPivotTable()
```


Gets the name of "Row Labels" label in the PivotTable.

**Remarks**

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.lang.String - The name of row labels
### getRowSeparatorOfFormulaArray() {#getRowSeparatorOfFormulaArray--}
```
public char getRowSeparatorOfFormulaArray()
```


Gets the separator for rows in array data in formula.

**Returns:**
char
### getStandardBuiltInName(String localName) {#getStandardBuiltInName-java.lang.String-}
```
public String getStandardBuiltInName(String localName)
```


Gets the standard text of built-in Name according to given locale dependent text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| localName | java.lang.String | Locale dependent text of built-in Name. The locale was specified by the Workbook for which this settings is used. |

**Returns:**
java.lang.String - Standard(en-US locale) text.
### getStandardFunctionName(String localName) {#getStandardFunctionName-java.lang.String-}
```
public String getStandardFunctionName(String localName)
```


Gets the standard function name according to given locale dependent function name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| localName | java.lang.String | Locale dependent function name. The locale was specified by the Workbook for which this settings is used. |

**Returns:**
java.lang.String - Standard(en-US locale) function name.
### getStandardHeaderFooterFontStyleName(String localfontStyleName) {#getStandardHeaderFooterFontStyleName-java.lang.String-}
```
public String getStandardHeaderFooterFontStyleName(String localfontStyleName)
```


Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| localfontStyleName | java.lang.String | Locale font style name for Header/Footer. |

**Returns:**
java.lang.String - Standard English font style name(Regular, Bold, Italic)
### getSubTotalName(int subTotalType) {#getSubTotalName-int-}
```
public String getSubTotalName(int subTotalType)
```


Gets the name of [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) type in the PivotTable.

**Remarks**

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). The [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) type |

**Returns:**
java.lang.String - The name of [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) type
### getTableRowTypeOfAll() {#getTableRowTypeOfAll--}
```
public String getTableRowTypeOfAll()
```


Gets the type name of table rows that consists of all rows in referenced table.

**Returns:**
java.lang.String - the type name of table rows
### getTableRowTypeOfCurrent() {#getTableRowTypeOfCurrent--}
```
public String getTableRowTypeOfCurrent()
```


Gets the type name of table rows that consists of the current row in referenced table.

**Returns:**
java.lang.String - the type name of table rows
### getTableRowTypeOfData() {#getTableRowTypeOfData--}
```
public String getTableRowTypeOfData()
```


Gets the type name of table rows that consists of data region of referenced table. Default is "Data", so in formula "\#Data" represents the data region of the table.

**Returns:**
java.lang.String - the type name of table rows
### getTableRowTypeOfHeaders() {#getTableRowTypeOfHeaders--}
```
public String getTableRowTypeOfHeaders()
```


Gets the type name of table rows that consists of the table header. Default is "Headers", so in formula "\#Headers" represents the table header.

**Returns:**
java.lang.String - the type name of table rows
### getTableRowTypeOfTotals() {#getTableRowTypeOfTotals--}
```
public String getTableRowTypeOfTotals()
```


Gets the type name of table rows that consists of the total row of referenced table.

**Returns:**
java.lang.String - the type name of table rows
### getTotalName(int functionType) {#getTotalName-int-}
```
public String getTotalName(int functionType)
```


Gets the total name of specific function.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). The function type. |

**Returns:**
java.lang.String - The total name of the function.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBooleanValueString(boolean bv, String name) {#setBooleanValueString-boolean-java.lang.String-}
```
public void setBooleanValueString(boolean bv, String name)
```


Sets the display string value for cell's boolean value

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| bv | boolean | boolean value |
| name | java.lang.String | string value of the boolean value |

### setChartSettings(ChartGlobalizationSettings value) {#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-}
```
public void setChartSettings(ChartGlobalizationSettings value)
```


Sets the globalization settings for Chart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings) |  |

### setColumnSeparatorOfFormulaArray(char c) {#setColumnSeparatorOfFormulaArray-char-}
```
public void setColumnSeparatorOfFormulaArray(char c)
```


Sets the separator for the items in array's row data in formula.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| c | char | the specified separator |

### setCommentTitleName(int type, String name) {#setCommentTitleName-int-java.lang.String-}
```
public void setCommentTitleName(int type, String name)
```


Gets the locale dependent comment title name according to comment title type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [CommentTitleType](../../com.aspose.cells/commenttitletype). type of comment title |
| name | java.lang.String | locale dependent comment title name |

### setGrandTotalName(int functionType, String name) {#setGrandTotalName-int-java.lang.String-}
```
public void setGrandTotalName(int functionType, String name)
```


Sets the grand total name of specific function.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). The function type. |
| name | java.lang.String | The grand total name of the function. |

### setListSeparator(char c) {#setListSeparator-char-}
```
public void setListSeparator(char c)
```


Sets the separator for list, parameters of function, ...etc.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| c | char | the specified separator |

### setLocalBuiltInName(String standardName, String localName, boolean bidirectional) {#setLocalBuiltInName-java.lang.String-java.lang.String-boolean-}
```
public void setLocalBuiltInName(String standardName, String localName, boolean bidirectional)
```


Sets the locale dependent text for the built-in name with given standard name text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| standardName | java.lang.String | Standard(en-US locale) name text of built-in name. |
| localName | java.lang.String | Locale dependent name text |
| bidirectional | boolean | Whether map the local name text to standard name text automatically. If true, the local name text will be mapped to standard name text automatically so user does not need to call [setStandardBuiltInName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setStandardBuiltInName-String-String-boolean-) again for the same standard and local names pair |

### setLocalFunctionName(String standardName, String localName, boolean bidirectional) {#setLocalFunctionName-java.lang.String-java.lang.String-boolean-}
```
public void setLocalFunctionName(String standardName, String localName, boolean bidirectional)
```


Sets the locale dependent function name corresponding to given standard function name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| standardName | java.lang.String | Standard(en-US locale) function name. |
| localName | java.lang.String | Locale dependent function name |
| bidirectional | boolean | Whether map the local function name to standard function name automatically. If true, the local name will be mapped to standard name automatically so user does not need to call [setStandardFunctionName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setStandardFunctionName-String-String-boolean-) again for the same standard and local names pair |

### setPivotSettings(PivotGlobalizationSettings value) {#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-}
```
public void setPivotSettings(PivotGlobalizationSettings value)
```


Sets the globalization settings for the pivot table.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings) |  |

### setRowSeparatorOfFormulaArray(char c) {#setRowSeparatorOfFormulaArray-char-}
```
public void setRowSeparatorOfFormulaArray(char c)
```


Sets the separator for rows in array data in formula.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| c | char | the specified separator |

### setStandardBuiltInName(String localName, String standardName, boolean bidirectional) {#setStandardBuiltInName-java.lang.String-java.lang.String-boolean-}
```
public void setStandardBuiltInName(String localName, String standardName, boolean bidirectional)
```


Sets the locale dependent function name according to given standard function name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| localName | java.lang.String | Locale dependent function name |
| standardName | java.lang.String | Standard(en-US locale) function name. |
| bidirectional | boolean | Whether map the standard name text to local name text automatically. If true, the standar name text will be mapped to local name text automatically so user does not need to call [setLocalBuiltInName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setLocalBuiltInName-String-String-boolean-) again for the same standard and local names pair |

### setStandardFunctionName(String localName, String standardName, boolean bidirectional) {#setStandardFunctionName-java.lang.String-java.lang.String-boolean-}
```
public void setStandardFunctionName(String localName, String standardName, boolean bidirectional)
```


Sets the locale dependent function name according to given standard function name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| localName | java.lang.String | Locale dependent function name |
| standardName | java.lang.String | Standard(en-US locale) function name. |
| bidirectional | boolean | Whether map the standard function name to local function name automatically. If true, the standar name will be mapped to local name automatically so user does not need to call [setLocalFunctionName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setLocalFunctionName-String-String-boolean-) again for the same standard and local names pair |

### setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName) {#setStandardHeaderFooterFontStyleName-java.lang.String-java.lang.String-}
```
public void setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName)
```


Sets the locale dependent function name according to given standard function name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| localfontStyleName | java.lang.String | Locale font style name for Header/Footer. |
| standardName | java.lang.String | Standard(en-US locale) function name. |

### setTableRowTypeOfAll(String name) {#setTableRowTypeOfAll-java.lang.String-}
```
public void setTableRowTypeOfAll(String name)
```


Sets the type name of table rows that consists of all rows in referenced table.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the type name of table rows |

### setTableRowTypeOfCurrent(String name) {#setTableRowTypeOfCurrent-java.lang.String-}
```
public void setTableRowTypeOfCurrent(String name)
```


Sets the type name of table rows that consists of the current row in referenced table.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the type name of table rows |

### setTableRowTypeOfData(String name) {#setTableRowTypeOfData-java.lang.String-}
```
public void setTableRowTypeOfData(String name)
```


Sets the type name of table rows that consists of data region of referenced table.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the type name of table rows |

### setTableRowTypeOfHeaders(String name) {#setTableRowTypeOfHeaders-java.lang.String-}
```
public void setTableRowTypeOfHeaders(String name)
```


Sets the type name of table rows that consists of the table header.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the type name of table rows |

### setTableRowTypeOfTotals(String name) {#setTableRowTypeOfTotals-java.lang.String-}
```
public void setTableRowTypeOfTotals(String name)
```


Sets the type name of table rows that consists of the total row of referenced table.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the type name of table rows |

### setTotalName(int functionType, String name) {#setTotalName-int-java.lang.String-}
```
public void setTotalName(int functionType, String name)
```


Sets the total name of specific function.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). The function type. |
| name | java.lang.String | The total name of the function. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

