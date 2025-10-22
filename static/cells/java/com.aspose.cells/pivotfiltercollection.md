##PivotFilterCollection
Represents a collection of all the PivotFilter objects
**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotFilterCollection extends CollectionBase
```
Represents a collection of all the PivotFilter objects
## Methods
| Method | Description |
| --- | --- |
| [add(int fieldIndex, int type)](#add-int-int-) | Adds a PivotFilter Object to the specific type |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2)](#addDateFilter-int-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-) | Filters by date setting of row or column pivot field. |
| [addLabelFilter(int baseFieldIndex, int type, String label1, String label2)](#addLabelFilter-int-int-java.lang.String-java.lang.String-) | Filters by captions of row or column pivot field. |
| [addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount)](#addTop10Filter-int-int-int-boolean-int-) | Filters by values of data pivot field. |
| [addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2)](#addValueFilter-int-int-int-double-double-) | Filters by values of data pivot field. |
| [clear()](#clear--) | Removes all objects from the CollectionBase instance. |
| [clearFilter(int fieldIndex)](#clearFilter-int-) | Clear PivotFilter from the specific PivotField |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the pivotfilter object at the specific index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Removes the item at the specified index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int fieldIndex, int type) {#add-int-int-}
```
public int add(int fieldIndex, int type)
```
Adds a PivotFilter Object to the specific type
**Remarks**
NOTE: This method is now obsolete. Instead, please use PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() and AddDateFilter() methods. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | the PivotField index |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). the PivotFilter type |
**Returns:**
int - the index of the PivotFilter Object in this PivotFilterCollection.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```
Adds an item to the CollectionBase instance.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | The Object to add to the CollectionBase instance. |
**Returns:**
int - The position into which the new element was inserted.
### addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2) {#addDateFilter-int-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-}
```
public PivotFilter addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2)
```
Filters by date setting of row or column pivot field.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | int | The index of field in the source. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). The type of filtering data. |
| dateTime1 | [DateTime](../../com.aspose.cells/datetime) | The date label of filter condition |
| dateTime2 | [DateTime](../../com.aspose.cells/datetime) | The upper-bound date label of between filter condition |
**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addLabelFilter(int baseFieldIndex, int type, String label1, String label2) {#addLabelFilter-int-int-java.lang.String-java.lang.String-}
```
public PivotFilter addLabelFilter(int baseFieldIndex, int type, String label1, String label2)
```
Filters by captions of row or column pivot field.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | int | The index of field in the source. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). The type of filtering data. |
| label1 | java.lang.String | The label of filter condition |
| label2 | java.lang.String | The upper-bound label of between filter condition |
**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount) {#addTop10Filter-int-int-int-boolean-int-}
```
public PivotFilter addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount)
```
Filters by values of data pivot field.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | int | The index of field in the source. |
| valueFieldIndex | int | The index of data field in the data region. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). The type of filtering data. Only can be Count,Sum and Percent. |
| isTop | boolean | Indicates whether filter from top or bottom |
| itemCount | int | The item count |
**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2) {#addValueFilter-int-int-int-double-double-}
```
public PivotFilter addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2)
```
Filters by values of data pivot field.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | int | The index of field in the source. |
| valueFieldIndex | int | The index of value field in the value region. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). The type of filtering data. |
| value1 | double | The value of filter condition |
| value2 | double | The upper-bound value of between filter condition |
**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### clear() {#clear--}
```
public void clear()
```
Removes all objects from the CollectionBase instance.
### clearFilter(int fieldIndex) {#clearFilter-int-}
```
public void clearFilter(int fieldIndex)
```
Clear PivotFilter from the specific PivotField
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | the PivotField index |
### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```
Return whether instance contains this object
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | test object |
**Returns:**
boolean - Whether instance contains this object
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
### get(int index) {#get-int-}
```
public PivotFilter get(int index)
```
Gets the pivotfilter object at the specific index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |
**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```
Gets the number of elements contained in the CollectionBase instance.
**Returns:**
int - The number of elements contained in the CollectionBase instance.
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```
Determines the index of a specific item in the CollectionBase instance.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | Determines the index of a specific item in the CollectionBase instance. |
**Returns:**
int - The index of value if found in the list; otherwise, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```
Returns an enumerator that iterates through the CollectionBase instance.
**Returns:**
java.util.Iterator - An iterator for the CollectionBase instance.
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```
Removes the item at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero-based index of the item to remove. |
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
