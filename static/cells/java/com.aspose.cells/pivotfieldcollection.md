##PivotFieldCollection
Represents a collection of all the PivotField objects in the PivotTables specific PivotFields type.
**Inheritance:**
java.lang.Object
**All Implemented Interfaces:**
java.lang.Iterable
```
public class PivotFieldCollection implements Iterable
```
Represents a collection of all the PivotField objects in the PivotTable's specific PivotFields type.
## Methods
| Method | Description |
| --- | --- |
| [add(PivotField pivotField)](#add-com.aspose.cells.PivotField-) | Adds a PivotField Object to the specific type PivotFields. |
| [addByBaseIndex(int baseFieldIndex)](#addByBaseIndex-int-) | Adds a PivotField Object to the specific type PivotFields. |
| [clear()](#clear--) | clear all fields of PivotFieldCollection |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the PivotField Object at the specific index. |
| [get(String name)](#get-java.lang.String-) | Gets the PivotField Object of the specific name. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the count of the pivotFields. |
| [getType()](#getType--) | Gets the PivotFields type. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Gets an enumerator over the elements in this collection in proper sequence. |
| [move(int currPos, int destPos)](#move-int-int-) | Moves the PivotField from current position to destination position |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(PivotField pivotField) {#add-com.aspose.cells.PivotField-}
```
public int add(PivotField pivotField)
```
Adds a PivotField Object to the specific type PivotFields.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | a PivotField Object. |
**Returns:**
int - the index of the PivotField Object in this PivotFields.
### addByBaseIndex(int baseFieldIndex) {#addByBaseIndex-int-}
```
public int addByBaseIndex(int baseFieldIndex)
```
Adds a PivotField Object to the specific type PivotFields.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | int | field index in the base PivotFields. |
**Returns:**
int - the index of the PivotField Object in this PivotFields.
### clear() {#clear--}
```
public void clear()
```
clear all fields of PivotFieldCollection
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
public PivotField get(int index)
```
Gets the PivotField Object at the specific index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |
**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### get(String name) {#get-java.lang.String-}
```
public PivotField get(String name)
```
Gets the PivotField Object of the specific name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |
**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
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
Gets the count of the pivotFields.
**Returns:**
int
### getType() {#getType--}
```
public int getType()
```
Gets the PivotFields type.
See [PivotFieldType](../../com.aspose.cells/pivotfieldtype).
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```
Gets an enumerator over the elements in this collection in proper sequence.
**Returns:**
java.util.Iterator - enumerator
### move(int currPos, int destPos) {#move-int-int-}
```
public void move(int currPos, int destPos)
```
Moves the PivotField from current position to destination position
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| currPos | int | Current position of PivotField based on zero |
| destPos | int | Destination position of PivotField based on zero |
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
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
