##DocumentPropertyCollection
Base class for  and  collections.
**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public abstract class DocumentPropertyCollection extends CollectionBase
```
Base class for [BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection) and [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) collections.
**Example**
```
//Instantiate a Workbook object by calling its empty constructor
Workbook workbook = new Workbook("book1.xls");
//Retrieve a list of all custom document properties of the Excel file
DocumentPropertyCollection customProperties = workbook.getWorksheets().getCustomDocumentProperties();
//Accessng a custom document property by using the property index
DocumentProperty customProperty1 = customProperties.get(3);
//Accessng a custom document property by using the property name
DocumentProperty customProperty2 = customProperties.get("Owner");
```
## Methods
| Method | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [clear()](#clear--) | Removes all objects from the CollectionBase instance. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [contains(String name)](#contains-java.lang.String-) | Returns true if a property with the specified name exists in the collection. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Returns a [DocumentProperty](../../com.aspose.cells/documentproperty) object by index. |
| [get(String name)](#get-java.lang.String-) | Returns a [DocumentProperty](../../com.aspose.cells/documentproperty) object by the name of the property. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [indexOf(String name)](#indexOf-java.lang.String-) | Gets the index of a property by name. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String name)](#remove-java.lang.String-) | Removes a property with the specified name from the collection. |
| [removeAt(int index)](#removeAt-int-) | Removes a property at the specified index. |
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
### contains(String name) {#contains-java.lang.String-}
```
public boolean contains(String name)
```
Returns true if a property with the specified name exists in the collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The case-insensitive name of the property. |
**Returns:**
boolean - True if the property exists in the collection; false otherwise.
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
public DocumentProperty get(int index)
```
Returns a [DocumentProperty](../../com.aspose.cells/documentproperty) object by index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | Zero-based index of the [DocumentProperty](../../com.aspose.cells/documentproperty) to retrieve. |
**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### get(String name) {#get-java.lang.String-}
```
public DocumentProperty get(String name)
```
Returns a [DocumentProperty](../../com.aspose.cells/documentproperty) object by the name of the property.
**Remarks**
Returns null if a property with the specified name is not found.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The case-insensitive name of the property to retrieve. |
**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
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
### indexOf(String name) {#indexOf-java.lang.String-}
```
public int indexOf(String name)
```
Gets the index of a property by name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The case-insensitive name of the property. |
**Returns:**
int - The zero based index. Negative value if not found.
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
### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```
Removes a property with the specified name from the collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The case-insensitive name of the property. |
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```
Removes a property at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index. |
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
