---
title: GlobalizationSettings
second_title: Aspose.Cells for Java API Reference
description: Represents the globalization settings.
type: docs
weight: 240
url: /java/com.aspose.cells/globalizationsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractGlobalizationSettings](../../com.aspose.cells/abstractglobalizationsettings)
```
public class GlobalizationSettings extends AbstractGlobalizationSettings
```

Represents the globalization settings.
## Methods

| Method | Description |
| --- | --- |
| [compare(String v1, String v2, boolean ignoreCase)](#compare-java.lang.String-java.lang.String-boolean-) | Compares two string values according to certain collation rules. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllName()](#getAllName--) | Gets the name of "(All)" label in the PivotTable. |
| [getBooleanValueString(boolean bv)](#getBooleanValueString-boolean-) | Gets the display string value for cell's boolean value |
| [getChartSettings()](#getChartSettings--) | the Chart of this[ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings) |
| [getClass()](#getClass--) |  |
| [getCollationKey(String v, boolean ignoreCase)](#getCollationKey-java.lang.String-boolean-) | Transforms the string into a comparable object according to certain collation rules. |
| [getColumnLabelsOfPivotTable()](#getColumnLabelsOfPivotTable--) | Gets the name of "Column Labels" label in the PivotTable. |
| [getColumnLablesName()](#getColumnLablesName--) | Gets the name of "Column Labels" label in the PivotTable. |
| [getColumnSeparatorOfFormulaArray()](#getColumnSeparatorOfFormulaArray--) | Gets the separator for the items in array's row data in formula. |
| [getCommentTitleName(int type)](#getCommentTitleName-int-) | Gets the locale dependent comment title name according to comment title type. |
| [getEmptyDataName()](#getEmptyDataName--) | Gets the name of "(blank)" label in the PivotTable. |
| [getErrorValueString(String err)](#getErrorValueString-java.lang.String-) | Gets the display string value for cell's error value |
| [getGrandTotalName(int functionType)](#getGrandTotalName-int-) | Gets the grand total name of the function. |
| [getListSeparator()](#getListSeparator--) | Gets the separator for list, parameters of function, ...etc. |
| [getLocalBuiltInName(String standardName)](#getLocalBuiltInName-java.lang.String-) | Gets the locale dependent text for built-in Name according to given standard text. |
| [getLocalFunctionName(String standardName)](#getLocalFunctionName-java.lang.String-) | Gets the locale dependent function name according to given standard function name. |
| [getMultipleItemsName()](#getMultipleItemsName--) | Gets the name of "(Multiple Items)" label in the PivotTable. |
| [getOtherName()](#getOtherName--) | Gets the name of "Other" labels for Pie charts. |
| [getPivotGrandTotalName()](#getPivotGrandTotalName--) | Gets the name of "Grand Total" label in the PivotTable. |
| [getPivotTotalName()](#getPivotTotalName--) | Gets the name of "Total" label in the PivotTable. |
| [getProtectionNameOfPivotTable()](#getProtectionNameOfPivotTable--) | Gets the protection name in the PivotTable. |
| [getRowLabelsNameOfPivotTable()](#getRowLabelsNameOfPivotTable--) | Gets the name of "Row Labels" label in the PivotTable. |
| [getRowLablesName()](#getRowLablesName--) | Gets the name of "Row Labels" label in the PivotTable. |
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
| [getTotalName(int functionType)](#getTotalName-int-) | Gets the total name of the function. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setChartSettings(ChartGlobalizationSettings value)](#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-) | For the description of this property, please see [getChartSettings()](../../com.aspose.cells/globalizationsettings\#getChartSettings--) |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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


Gets the name of "(All)" label in the PivotTable.

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
java.lang.String - Default returns "TRUE" for true value and "FALSE" for false value.
### getChartSettings() {#getChartSettings--}
```
public ChartGlobalizationSettings getChartSettings()
```


the Chart of this[ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings)

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


Gets the name of "Column Labels" label in the PivotTable.

**Returns:**
java.lang.String - The name of column labels
### getColumnLablesName() {#getColumnLablesName--}
```
public String getColumnLablesName()
```


Gets the name of "Column Labels" label in the PivotTable. NOTE: This member is now obsolete. Instead, please use GlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since September 2020. Aspose apologizes for any inconvenience you may have experienced.

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
| type | int |  |

**Returns:**
java.lang.String - 
### getEmptyDataName() {#getEmptyDataName--}
```
public String getEmptyDataName()
```


Gets the name of "(blank)" label in the PivotTable.

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
java.lang.String - Default returns the error value itself
### getGrandTotalName(int functionType) {#getGrandTotalName-int-}
```
public String getGrandTotalName(int functionType)
```


Gets the grand total name of the function.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| functionType | int | The function type. |

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


Gets the name of "(Multiple Items)" label in the PivotTable.

**Returns:**
java.lang.String - The name of "(Multiple Items)" label
### getOtherName() {#getOtherName--}
```
public String getOtherName()
```


Gets the name of "Other" labels for Pie charts.

**Returns:**
java.lang.String - 
### getPivotGrandTotalName() {#getPivotGrandTotalName--}
```
public String getPivotGrandTotalName()
```


Gets the name of "Grand Total" label in the PivotTable.

**Returns:**
java.lang.String - The name of "Grand Total" label
### getPivotTotalName() {#getPivotTotalName--}
```
public String getPivotTotalName()
```


Gets the name of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area.

**Returns:**
java.lang.String - The name of "Total" label
### getProtectionNameOfPivotTable() {#getProtectionNameOfPivotTable--}
```
public String getProtectionNameOfPivotTable()
```


Gets the protection name in the PivotTable.

**Returns:**
java.lang.String - The protection name of PivotTable
### getRowLabelsNameOfPivotTable() {#getRowLabelsNameOfPivotTable--}
```
public String getRowLabelsNameOfPivotTable()
```


Gets the name of "Row Labels" label in the PivotTable.

**Returns:**
java.lang.String - The name of row labels
### getRowLablesName() {#getRowLablesName--}
```
public String getRowLablesName()
```


Gets the name of "Row Labels" label in the PivotTable. NOTE: This member is now obsolete. Instead, please use GlobalizationSettings.GetRowLabelsOfPivotTable() method. This property will be removed 12 months later since September 2020. Aspose apologizes for any inconvenience you may have experienced.

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

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subTotalType | int | The [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) type |

**Returns:**
java.lang.String - The name of [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) type
### getTableRowTypeOfAll() {#getTableRowTypeOfAll--}
```
public String getTableRowTypeOfAll()
```


Gets the type name of table rows that consists of all rows in referenced table. Default is "All", so in formula "\#All" represents all rows in referenced table.

**Returns:**
java.lang.String - the type name of table rows
### getTableRowTypeOfCurrent() {#getTableRowTypeOfCurrent--}
```
public String getTableRowTypeOfCurrent()
```


Gets the type name of table rows that consists of the current row in referenced table. Default is "This Row", so in formula "\#This Row" represents the current row in referenced table.

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


Gets the type name of table rows that consists of the total row of referenced table. Default is "Totals", so in formula "\#Totals" represents the total row of referenced table.

**Returns:**
java.lang.String - the type name of table rows
### getTotalName(int functionType) {#getTotalName-int-}
```
public String getTotalName(int functionType)
```


Gets the total name of the function.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| functionType | int | The function type. |

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




### setChartSettings(ChartGlobalizationSettings value) {#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-}
```
public void setChartSettings(ChartGlobalizationSettings value)
```


For the description of this property, please see [getChartSettings()](../../com.aspose.cells/globalizationsettings\#getChartSettings--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings) |  |

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

