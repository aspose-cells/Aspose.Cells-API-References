---
title: SettablePivotGlobalizationSettings
second_title: Aspose.Cells for Java API Reference
description: Implementation of PivotGlobalizationSettings that supports user to set/change pre-defined texts.
type: docs
url: /java/com.aspose.cells/settablepivotglobalizationsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)
```
public class SettablePivotGlobalizationSettings extends PivotGlobalizationSettings
```

Implementation of PivotGlobalizationSettings that supports user to set/change pre-defined texts.
## Constructors

| Constructor | Description |
| --- | --- |
| [SettablePivotGlobalizationSettings()](#SettablePivotGlobalizationSettings--) |  |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getTextOfAll()](#getTextOfAll--) | Gets the text of "(All)" label in the PivotTable. |
| [getTextOfColumnLabels()](#getTextOfColumnLabels--) | Gets the text of "Column Labels" label in the PivotTable. |
| [getTextOfDataFieldHeader()](#getTextOfDataFieldHeader--) | Gets the the text of the value area field header in the PivotTable. |
| [getTextOfEmptyData()](#getTextOfEmptyData--) | Gets the text of "(blank)" label in the PivotTable. |
| [getTextOfGrandTotal()](#getTextOfGrandTotal--) | Gets the text of "Grand Total" label in the PivotTable. |
| [getTextOfMultipleItems()](#getTextOfMultipleItems--) | Gets the text of "(Multiple Items)" label in the PivotTable. |
| [getTextOfProtectedName(String protectedName)](#getTextOfProtectedName-java.lang.String-) | Gets the text for specified protected name. |
| [getTextOfProtection()](#getTextOfProtection--) | Gets the protection name in the PivotTable. |
| [getTextOfRowLabels()](#getTextOfRowLabels--) | Gets the text of "Row Labels" label in the PivotTable. |
| [getTextOfSubTotal(int subTotalType)](#getTextOfSubTotal-int-) | Gets the text of [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) type in the PivotTable. |
| [getTextOfTotal()](#getTextOfTotal--) | Gets the text of "Total" label in the PivotTable. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setTextOfAll(String text)](#setTextOfAll-java.lang.String-) | Sets the text of "(All)" label in the PivotTable. |
| [setTextOfColumnLabels(String text)](#setTextOfColumnLabels-java.lang.String-) | Gets the text of "Column Labels" label in the PivotTable. |
| [setTextOfDataFieldHeader(String text)](#setTextOfDataFieldHeader-java.lang.String-) | Sets the the text of the value area field header in the PivotTable. |
| [setTextOfEmptyData(String text)](#setTextOfEmptyData-java.lang.String-) | Sets the text of "(blank)" label in the PivotTable. |
| [setTextOfGrandTotal(String text)](#setTextOfGrandTotal-java.lang.String-) | Sets the text of "Grand Total" label in the PivotTable. |
| [setTextOfMultipleItems(String text)](#setTextOfMultipleItems-java.lang.String-) | Sets the text of "(Multiple Items)" label in the PivotTable. |
| [setTextOfProtectedName(String protectedName, String text)](#setTextOfProtectedName-java.lang.String-java.lang.String-) | Sets the text for specific protected name. |
| [setTextOfRowLabels(String text)](#setTextOfRowLabels-java.lang.String-) | Sets the text of "Row Labels" label in the PivotTable. |
| [setTextOfSubTotal(int subTotalType, String text)](#setTextOfSubTotal-int-java.lang.String-) | Sets the text of [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) type in the PivotTable. |
| [setTextOfTotal(String text)](#setTextOfTotal-java.lang.String-) | Sets the text of "Total" label in the PivotTable. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SettablePivotGlobalizationSettings() {#SettablePivotGlobalizationSettings--}
```
public SettablePivotGlobalizationSettings()
```


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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getTextOfAll() {#getTextOfAll--}
```
public String getTextOfAll()
```


Gets the text of "(All)" label in the PivotTable.

**Returns:**
java.lang.String - The text of "(All)" label
### getTextOfColumnLabels() {#getTextOfColumnLabels--}
```
public String getTextOfColumnLabels()
```


Gets the text of "Column Labels" label in the PivotTable.

**Returns:**
java.lang.String - The text of column labels
### getTextOfDataFieldHeader() {#getTextOfDataFieldHeader--}
```
public String getTextOfDataFieldHeader()
```


Gets the the text of the value area field header in the PivotTable.

**Returns:**
java.lang.String - The text of data field header name
### getTextOfEmptyData() {#getTextOfEmptyData--}
```
public String getTextOfEmptyData()
```


Gets the text of "(blank)" label in the PivotTable.

**Returns:**
java.lang.String - The text of empty data
### getTextOfGrandTotal() {#getTextOfGrandTotal--}
```
public String getTextOfGrandTotal()
```


Gets the text of "Grand Total" label in the PivotTable.

**Returns:**
java.lang.String - The text of "Grand Total" label
### getTextOfMultipleItems() {#getTextOfMultipleItems--}
```
public String getTextOfMultipleItems()
```


Gets the text of "(Multiple Items)" label in the PivotTable.

**Returns:**
java.lang.String - The text of "(Multiple Items)" label
### getTextOfProtectedName(String protectedName) {#getTextOfProtectedName-java.lang.String-}
```
public String getTextOfProtectedName(String protectedName)
```


Gets the text for specified protected name.

**Remarks**

In Ms Excel, some names are not allowed to be used as the name of PivotFields in PivotTable. They are different in different region, user may specify them explicitly according to the used region.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| protectedName | java.lang.String | The protected name in PivotTable. |

**Returns:**
java.lang.String - The local prorected names of PivotTable.
### getTextOfProtection() {#getTextOfProtection--}
```
public String getTextOfProtection()
```


Gets the protection name in the PivotTable.

**Remarks**

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetTextOfProtectedName(string) method. This property will be removed 12 months later since March 2023. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.lang.String - The protection name of PivotTable
### getTextOfRowLabels() {#getTextOfRowLabels--}
```
public String getTextOfRowLabels()
```


Gets the text of "Row Labels" label in the PivotTable.

**Returns:**
java.lang.String - The text of row labels
### getTextOfSubTotal(int subTotalType) {#getTextOfSubTotal-int-}
```
public String getTextOfSubTotal(int subTotalType)
```


Gets the text of [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) type in the PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). The [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |

**Returns:**
java.lang.String - The text of given type
### getTextOfTotal() {#getTextOfTotal--}
```
public String getTextOfTotal()
```


Gets the text of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area.

**Returns:**
java.lang.String - The text of "Total" label
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




### setTextOfAll(String text) {#setTextOfAll-java.lang.String-}
```
public void setTextOfAll(String text)
```


Sets the text of "(All)" label in the PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | custom text |

### setTextOfColumnLabels(String text) {#setTextOfColumnLabels-java.lang.String-}
```
public void setTextOfColumnLabels(String text)
```


Gets the text of "Column Labels" label in the PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | The text of column labels |

### setTextOfDataFieldHeader(String text) {#setTextOfDataFieldHeader-java.lang.String-}
```
public void setTextOfDataFieldHeader(String text)
```


Sets the the text of the value area field header in the PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | The text of data field header name |

### setTextOfEmptyData(String text) {#setTextOfEmptyData-java.lang.String-}
```
public void setTextOfEmptyData(String text)
```


Sets the text of "(blank)" label in the PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | The text of empty data |

### setTextOfGrandTotal(String text) {#setTextOfGrandTotal-java.lang.String-}
```
public void setTextOfGrandTotal(String text)
```


Sets the text of "Grand Total" label in the PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | custom text |

### setTextOfMultipleItems(String text) {#setTextOfMultipleItems-java.lang.String-}
```
public void setTextOfMultipleItems(String text)
```


Sets the text of "(Multiple Items)" label in the PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | custom text |

### setTextOfProtectedName(String protectedName, String text) {#setTextOfProtectedName-java.lang.String-java.lang.String-}
```
public void setTextOfProtectedName(String protectedName, String text)
```


Sets the text for specific protected name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| protectedName | java.lang.String | The protected name in PivotTable. |
| text | java.lang.String | The local prorected names of PivotTable. |

### setTextOfRowLabels(String text) {#setTextOfRowLabels-java.lang.String-}
```
public void setTextOfRowLabels(String text)
```


Sets the text of "Row Labels" label in the PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | The text of row labels |

### setTextOfSubTotal(int subTotalType, String text) {#setTextOfSubTotal-int-java.lang.String-}
```
public void setTextOfSubTotal(int subTotalType, String text)
```


Sets the text of [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) type in the PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). The [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |
| text | java.lang.String | The text of given type |

### setTextOfTotal(String text) {#setTextOfTotal-java.lang.String-}
```
public void setTextOfTotal(String text)
```


Sets the text of "Total" label in the PivotTable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | custom text |

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

