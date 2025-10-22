##CustomCommandButtonCollection
Represents the collection of CustomCommandButton.
**Inheritance:**
java.lang.Object, [com.aspose.gridweb.CollectionBase](../../com.aspose.gridweb/collectionbase)
```
public class CustomCommandButtonCollection extends CollectionBase
```
Represents the collection of CustomCommandButton.
**Example**
```
GridWeb GridWeb1 = new GridWeb();
CustomCommandButton button = new CustomCommandButton();
button.setCommand("MyCommand");
button.setImageUrl("images/button1.gif");
GridWeb1.getCustomCommandButtons().add(button);
```
## Methods
| Method | Description |
| --- | --- |
| [add(Object value)](#add-java.lang.Object-) | Add a custom command button object to the collection. |
| [clear()](#clear--) | Clears the collection. |
| [contains(Object value)](#contains-java.lang.Object-) | Indicates whether the custom command button object is in the collection. |
| [copyTo(Object[] array, int index)](#copyTo-java.lang.Object---int-) | Copies the collection to an array. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets a custom command button object at the index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the count of the collection. |
| [getSyncRoot()](#getSyncRoot--) | Internal used only. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object value)](#indexOf-java.lang.Object-) | Gets the index of the button. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | Inserts a button at the index. |
| [isFixedSize()](#isFixedSize--) | Internal used only. |
| [isReadOnly()](#isReadOnly--) | Internal used only. |
| [isSynchronized()](#isSynchronized--) | Internal used only. |
| [iterator()](#iterator--) | Gets a IEnumerator object of the collection. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Object value)](#remove-java.lang.Object-) | Removes the custom command button object. |
| [removeAt(int index)](#removeAt-int-) | Removes at the index. |
| [set(int index, CustomCommandButton value)](#set-int-com.aspose.gridweb.CustomCommandButton-) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object value) {#add-java.lang.Object-}
```
public int add(Object value)
```
Add a custom command button object to the collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object | The custom command button object. |
**Returns:**
int - The index.
### clear() {#clear--}
```
public void clear()
```
Clears the collection.
### contains(Object value) {#contains-java.lang.Object-}
```
public boolean contains(Object value)
```
Indicates whether the custom command button object is in the collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object | Indicates whether the custom command button object is in the collection. |
**Returns:**
boolean - True of false.
### copyTo(Object[] array, int index) {#copyTo-java.lang.Object---int-}
```
public void copyTo(Object[] array, int index)
```
Copies the collection to an array.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| array | java.lang.Object[] | The array. |
| index | int | The start index of the array. |
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
public CustomCommandButton get(int index)
```
Gets a custom command button object at the index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |
**Returns:**
[CustomCommandButton](../../com.aspose.gridweb/customcommandbutton)
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
Gets the count of the collection.
**Returns:**
int
### getSyncRoot() {#getSyncRoot--}
```
public Object getSyncRoot()
```
Internal used only.
**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### indexOf(Object value) {#indexOf-java.lang.Object-}
```
public int indexOf(Object value)
```
Gets the index of the button.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object | The button object. |
**Returns:**
int - The index.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public void insert(int index, Object value)
```
Inserts a button at the index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | Index. |
| value | java.lang.Object | The CustomCommandButton object. |
### isFixedSize() {#isFixedSize--}
```
public boolean isFixedSize()
```
Internal used only.
**Returns:**
boolean
### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```
Internal used only.
**Returns:**
boolean
### isSynchronized() {#isSynchronized--}
```
public boolean isSynchronized()
```
Internal used only.
**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```
Gets a IEnumerator object of the collection.
**Returns:**
java.util.Iterator - The IEnumerator object.
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### remove(Object value) {#remove-java.lang.Object-}
```
public void remove(Object value)
```
Removes the custom command button object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object | The custom command button object. |
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```
Removes at the index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | Index. |
### set(int index, CustomCommandButton value) {#set-int-com.aspose.gridweb.CustomCommandButton-}
```
public void set(int index, CustomCommandButton value)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |
| value | [CustomCommandButton](../../com.aspose.gridweb/customcommandbutton) |  |
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
