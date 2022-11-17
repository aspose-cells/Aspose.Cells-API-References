---
title: CustomXmlPartCollection
second_title: Aspose.Cells for Java API Reference
description: Represents a Custom XML Data Storage Part custom XML data within a package.
type: docs
weight: 145
url: /java/com.aspose.cells/customxmlpartcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class CustomXmlPartCollection extends CollectionBase
```

Represents a Custom XML Data Storage Part (custom XML data within a package).
## Constructors

| Constructor | Description |
| --- | --- |
| [CustomXmlPartCollection()](#CustomXmlPartCollection--) |  |
## Methods

| Method | Description |
| --- | --- |
| [add(byte[] data, byte[] shemaData)](#add-byte---byte---) | Adds an item to the collection. |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [clear()](#clear--) | Removes all objects from the CollectionBase instance. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets an item at the specified index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Removes the item at the specified index. |
| [selectByID(String id)](#selectByID-java.lang.String-) | Gets an item by id. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomXmlPartCollection() {#CustomXmlPartCollection--}
```
public CustomXmlPartCollection()
```


### add(byte[] data, byte[] shemaData) {#add-byte---byte---}
```
public int add(byte[] data, byte[] shemaData)
```


Adds an item to the collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| data | byte[] | The XML content of this Custom XML Data Storage Part. |
| shemaData | byte[] | The set of XML schemas that are associated with this custom XML part. |

**Returns:**
int - 
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
public CustomXmlPart get(int index)
```


Gets an item at the specified index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index. |

**Returns:**
[CustomXmlPart](../../com.aspose.cells/customxmlpart) - 
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

### selectByID(String id) {#selectByID-java.lang.String-}
```
public CustomXmlPart selectByID(String id)
```


Gets an item by id.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| id | java.lang.String | Contains the GUID for the custom XML part. |

**Returns:**
[CustomXmlPart](../../com.aspose.cells/customxmlpart) - 
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
