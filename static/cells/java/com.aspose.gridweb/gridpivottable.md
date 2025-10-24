##GridPivotTable
Represents a PivotTable report on a worksheet.
**Inheritance:**
java.lang.Object
```
public class GridPivotTable
```
Represents a PivotTable report on a worksheet. The PivotTable object is a member of the [GridPivotTable](../../com.aspose.gridweb/gridpivottable) collection. The PivotTables collection contains all the PivotTable objects on a control.
## Methods
| Method | Description |
| --- | --- |
| [addFieldToArea(int fieldType, int baseFieldIndex)](#addFieldToArea-int-int-) | Adds the field to the specific area. |
| [addFieldToArea(int fieldType, String fieldName)](#addFieldToArea-int-java.lang.String-) | Adds the field to the specific area. |
| [calculateData()](#calculateData--) | Calculates pivottable's data to cells. |
| [clearAllFields()](#clearAllFields--) | clear all pivot fields. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fields(int fieldType)](#fields-int-) | Gets the specific fields by the field type. |
| [fields(String fieldName)](#fields-java.lang.String-) | Gets the specific field by the field name. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshData()](#refreshData--) | Refreshes pivottable's data and setting from it's data source. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addFieldToArea(int fieldType, int baseFieldIndex) {#addFieldToArea-int-int-}
```
public int addFieldToArea(int fieldType, int baseFieldIndex)
```
Adds the field to the specific area.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). The fields area type. |
| baseFieldIndex | int | The field index in the base fields. |
**Returns:**
int - The field position in the specific fields.
### addFieldToArea(int fieldType, String fieldName) {#addFieldToArea-int-java.lang.String-}
```
public int addFieldToArea(int fieldType, String fieldName)
```
Adds the field to the specific area.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). The fields area type. |
| fieldName | java.lang.String | The name in the base fields. |
**Returns:**
int - The field position in the specific fields.If there is no field named as it, return -1.
### calculateData() {#calculateData--}
```
public void calculateData()
```
Calculates pivottable's data to cells.
**Remarks**
Cell.Value in the pivot range could not return the correct result if the method is not been called. This method caclulates data with an inner pivot cache,not original data source. So if the data source is changed, please call RefreshData() method first.
### clearAllFields() {#clearAllFields--}
```
public void clearAllFields()
```
clear all pivot fields.
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
### fields(int fieldType) {#fields-int-}
```
public GridPivotFieldCollection fields(int fieldType)
```
Gets the specific fields by the field type.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). the field type. |
**Returns:**
[GridPivotFieldCollection](../../com.aspose.gridweb/gridpivotfieldcollection) - the specific fields
### fields(String fieldName) {#fields-java.lang.String-}
```
public GridPivotField fields(String fieldName)
```
Gets the specific field by the field name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | java.lang.String | the field name. |
**Returns:**
[GridPivotField](../../com.aspose.gridweb/gridpivotfield) - the specific field
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
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
### refreshData() {#refreshData--}
```
public void refreshData()
```
Refreshes pivottable's data and setting from it's data source.
**Remarks**
We will gather data from data source to a pivot cache ,then calcualte the data in the cache to the cells. This method is only used to gather all data to a pivot cache.
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
