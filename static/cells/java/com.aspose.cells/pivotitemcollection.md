##PivotItemCollection
Represents all the  objects in the PivotField.
**Inheritance:**
java.lang.Object
**All Implemented Interfaces:**
java.lang.Iterable
```
public class PivotItemCollection implements Iterable
```
Represents all the [PivotItem](../../com.aspose.cells/pivotitem) objects in the PivotField.
## Methods
| Method | Description |
| --- | --- |
| [changeitemsOrder(int sourceIndex, int destIndex)](#changeitemsOrder-int-int-) | Directly changes the orders of the two items. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the PivotItem Object at the specific index. |
| [get(String itemValue)](#get-java.lang.String-) | Gets the [PivotItem](../../com.aspose.cells/pivotitem) by the specific name. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the count of the pivot items. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Gets an enumerator over the elements in this collection in proper sequence. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [swapItem(int index1, int index2)](#swapItem-int-int-) | Directly swap two items. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### changeitemsOrder(int sourceIndex, int destIndex) {#changeitemsOrder-int-int-}
```
public void changeitemsOrder(int sourceIndex, int destIndex)
```
Directly changes the orders of the two items.
**Remarks**
NOTE: This method is now obsolete. Instead, please use PivotItemCollection.SwapItem() method. This method will be removed 12 months later since July 2024. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | int | The current index |
| destIndex | int | The dest index |
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
public PivotItem get(int index)
```
Gets the PivotItem Object at the specific index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |
**Returns:**
[PivotItem](../../com.aspose.cells/pivotitem)
### get(String itemValue) {#get-java.lang.String-}
```
public PivotItem get(String itemValue)
```
Gets the [PivotItem](../../com.aspose.cells/pivotitem) by the specific name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| itemValue | java.lang.String |  |
**Returns:**
[PivotItem](../../com.aspose.cells/pivotitem)
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
Gets the count of the pivot items.
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
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### swapItem(int index1, int index2) {#swapItem-int-int-}
```
public void swapItem(int index1, int index2)
```
Directly swap two items.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index1 | int |  |
| index2 | int |  |
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
