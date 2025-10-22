##ConditionalFormattingIconCollection
Represents  a collection of  objects.
**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ConditionalFormattingIconCollection extends CollectionBase
```
Represents a collection of [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) objects.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
Worksheet sheet = workbook.getWorksheets().get(0);
//Get Conditional Formatting
ConditionalFormattingCollection cformattings = sheet.getConditionalFormattings();
//Adds an empty conditional formatting
int index = cformattings.add();
//Get newly added Conditional formatting
FormatConditionCollection fcs = cformattings.get(index);
//Sets the conditional format range.
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 0;
ca.EndColumn = 0;
fcs.addArea(ca);
ca = new CellArea();
ca.StartRow = 1;
ca.EndRow = 1;
ca.StartColumn = 1;
ca.EndColumn = 1;
fcs.addArea(ca);
//Sets condition
int idx = fcs.addCondition(FormatConditionType.ICON_SET);
FormatCondition cond = fcs.get(idx);
//Sets condition's type
cond.getIconSet().setType(IconSetType.ARROWS_GRAY_3);
//Add custom iconset condition.
ConditionalFormattingIcon cfIcon = cond.getIconSet().getCfIcons().get(0);
cfIcon.setType(IconSetType.ARROWS_3);
cfIcon.setIndex(0);
ConditionalFormattingIcon cfIcon1 = cond.getIconSet().getCfIcons().get(1);
cfIcon1.setType(IconSetType.ARROWS_GRAY_3);
cfIcon1.setIndex(1);
ConditionalFormattingIcon cfIcon2 = cond.getIconSet().getCfIcons().get(2);
cfIcon2.setType(IconSetType.BOXES_5);
cfIcon2.setIndex(2);
//Saving the Excel file
workbook.save("output.xls");
```
## Methods
| Method | Description |
| --- | --- |
| [add(ConditionalFormattingIcon cficon)](#add-com.aspose.cells.ConditionalFormattingIcon-) | Adds [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) object. |
| [add(int type, int index)](#add-int-int-) | Adds [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) object. |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [clear()](#clear--) | Removes all objects from the CollectionBase instance. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the ConditionalFormattingIcon element at the specified index. |
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
### add(ConditionalFormattingIcon cficon) {#add-com.aspose.cells.ConditionalFormattingIcon-}
```
public int add(ConditionalFormattingIcon cficon)
```
Adds [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cficon | [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) | Returns the index of new object in the list. |
**Returns:**
int
### add(int type, int index) {#add-int-int-}
```
public int add(int type, int index)
```
Adds [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [IconSetType](../../com.aspose.cells/iconsettype). The value type. |
| index | int | The Index. |
**Returns:**
int - Returns the index of new object in the list.
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
### get(int index) {#get-int-}
```
public ConditionalFormattingIcon get(int index)
```
Gets the ConditionalFormattingIcon element at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
**Returns:**
[ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) - The element at the specified index.
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
