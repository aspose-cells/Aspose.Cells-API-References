##PivotTableFormatCollection
Represents the collection of formats applied to PivotTable.
**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotTableFormatCollection extends CollectionBase
```
Represents the collection of formats applied to PivotTable.
## Methods
| Method | Description |
| --- | --- |
| [add()](#add--) | Add a [PivotTableFormat](../../com.aspose.cells/pivottableformat). |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [clear()](#clear--) | Removes all objects from the CollectionBase instance. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [formatArea(int axisType, int fieldPosition, int subtotalType, int selectionType, boolean isGrandRow, boolean isGrandColumn, Style style)](#formatArea-int-int-int-int-boolean-boolean-com.aspose.cells.Style-) | Formats selected area. |
| [get(int index)](#get-int-) | Gets the format by the index. |
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
### add() {#add--}
```
public int add()
```
Add a [PivotTableFormat](../../com.aspose.cells/pivottableformat).
**Returns:**
int - The index of new format.
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
### clear() {#clear--}
```
public void clear()
```
Removes all objects from the CollectionBase instance.
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
### formatArea(int axisType, int fieldPosition, int subtotalType, int selectionType, boolean isGrandRow, boolean isGrandColumn, Style style) {#formatArea-int-int-int-int-boolean-boolean-com.aspose.cells.Style-}
```
public PivotTableFormat formatArea(int axisType, int fieldPosition, int subtotalType, int selectionType, boolean isGrandRow, boolean isGrandColumn, Style style)
```
Formats selected area.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). The region of the PivotTable to which this rule applies. |
| fieldPosition | int | Position of the field within the axis to which this rule applies. |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). The subtotal filter type of the pivot field |
| selectionType | int | [PivotTableSelectionType](../../com.aspose.cells/pivottableselectiontype). Indicates how to select data. |
| isGrandRow | boolean | Indicates whether selecting grand total rows. |
| isGrandColumn | boolean | Indicates whether selecting grand total columns. |
| style | [Style](../../com.aspose.cells/style) | The style which appies to the area of the pivot table. |
**Returns:**
[PivotTableFormat](../../com.aspose.cells/pivottableformat) -
### get(int index) {#get-int-}
```
public PivotTableFormat get(int index)
```
Gets the format by the index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index. |
**Returns:**
[PivotTableFormat](../../com.aspose.cells/pivottableformat) -
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
