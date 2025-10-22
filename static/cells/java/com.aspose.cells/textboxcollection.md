##TextBoxCollection
Encapsulates a collection of  objects.
**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TextBoxCollection extends CollectionBase
```
Encapsulates a collection of [TextBox](../../com.aspose.cells/textbox) objects.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
//get collection object
TextBoxCollection textBoxCollection = workbook.getWorksheets().get(0).getTextBoxes();
//add a textbox
textBoxCollection.add(1, 1, 50, 100);
for(TextBox tbox : (Iterable<TextBox>) textBoxCollection)
{
//do what you want
}
//do your business
```
## Methods
| Method | Description |
| --- | --- |
| [add(int upperLeftRow, int upperLeftColumn, int height, int width)](#add-int-int-int-int-) | Adds a textbox to the collection. |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [clear()](#clear--) | Clear all text boxes. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the [TextBox](../../com.aspose.cells/textbox) element at the specified index. |
| [get(String name)](#get-java.lang.String-) | Gets the [TextBox](../../com.aspose.cells/textbox) element by the name. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Remove a text box from the file. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int upperLeftRow, int upperLeftColumn, int height, int width) {#add-int-int-int-int-}
```
public int add(int upperLeftRow, int upperLeftColumn, int height, int width)
```
Adds a textbox to the collection.
**Example**
```
//add a TextBox
int index2 = textBoxCollection.add(1, 1, 50, 100);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int | Upper left row index. |
| upperLeftColumn | int | Upper left column index. |
| height | int | Height of textbox, in unit of pixel. |
| width | int | Width of textbox, in unit of pixel. |
**Returns:**
int - [TextBox](../../com.aspose.cells/textbox) object index.
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
Clear all text boxes.
**Example**
```
//clear all textbox
textBoxCollection.clear();
```
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
public TextBox get(int index)
```
Gets the [TextBox](../../com.aspose.cells/textbox) element at the specified index.
**Example**
```
int index = textBoxCollection.getCount() - 1;
TextBox txb = textBoxCollection.get(index);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
**Returns:**
[TextBox](../../com.aspose.cells/textbox) - The element at the specified index.
### get(String name) {#get-java.lang.String-}
```
public TextBox get(String name)
```
Gets the [TextBox](../../com.aspose.cells/textbox) element by the name.
**Example**
```
String txtboxName = "textbox 1";
TextBox txb2 = textBoxCollection.get(txtboxName);
if(txb2 != null)
{
//do what you want
}
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the text box. |
**Returns:**
[TextBox](../../com.aspose.cells/textbox) -
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
Remove a text box from the file.
**Example**
```
int index3 = textBoxCollection.getCount() - 1;
textBoxCollection.removeAt(index3);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The text box index. |
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
