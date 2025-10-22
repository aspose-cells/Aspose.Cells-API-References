##XmlMapCollection
A collection of  objects that represent XmlMap information.
**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class XmlMapCollection extends CollectionBase
```
A collection of [ListObject.getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--) objects that represent XmlMap information.
## Methods
| Method | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [add(String url)](#add-java.lang.String-) | Add a [ListObject.getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--) by the url/path of a xml/xsd file. |
| [clear()](#clear--) | Removes all XmlMaps. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the xml map by the specific index. |
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
### add(String url) {#add-java.lang.String-}
```
public int add(String url)
```
Add a [ListObject.getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--) by the url/path of a xml/xsd file.
**Example**
The following code adds two XmlMaps by a xsd file and a xml file.
```
Workbook wb = new Workbook();
XmlMapCollection xmlMapCollection = wb.getWorksheets().getXmlMaps();
//Add a XmlMap by a xsd file.
xmlMapCollection.add("schema.xsd");
//Add a XmlMap by a xml file.
xmlMapCollection.add("xml.xml");
wb.save("twoXmlMaps.xlsx");
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| url | java.lang.String | url/path of a xml/xsd file. |
**Returns:**
int - [ListObject.getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--) object index.
### clear() {#clear--}
```
public void clear()
```
Removes all XmlMaps.
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
public XmlMap get(int index)
```
Gets the xml map by the specific index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index. |
**Returns:**
[XmlMap](../../com.aspose.cells/xmlmap) - The xml map
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
