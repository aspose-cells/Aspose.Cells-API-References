---
title: PictureCollection
second_title: Aspose.Cells for Java API Reference
description: Encapsulates a collection of  objects.
type: docs
url: /java/com.aspose.cells/picturecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PictureCollection extends CollectionBase
```

Encapsulates a collection of [Picture](../../com.aspose.cells/picture) objects.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //get PictureCollection
         PictureCollection pictures = workbook.getWorksheets().get(0).getPictures();
 
         //do your business
 
         //Save the excel file.
         workbook.save("result.xlsx");
```
## Methods

| Method | Description |
| --- | --- |
| [add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)](#add-int-int-int-int-java.io.InputStream-) | Adds a picture to the collection. |
| [add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName)](#add-int-int-int-int-java.lang.String-) | Adds a picture to the collection. |
| [add(int topRow, int leftColumn, InputStream stream)](#add-int-int-java.io.InputStream-) | Adds a picture to the collection. |
| [add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)](#add-int-int-java.io.InputStream-int-int-) | Adds a picture to the collection. |
| [add(int topRow, int leftColumn, String fileName)](#add-int-int-java.lang.String-) | Adds a picture to the collection. |
| [add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale)](#add-int-int-java.lang.String-int-int-) | Adds a picture to the collection. |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [camera(int row, int column, String range)](#camera-int-int-java.lang.String-) | Takes a photo of the range. |
| [clear()](#clear--) | Clear all pictures. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the [Picture](../../com.aspose.cells/picture) element at the specified index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Remove shapes at the specific index |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream) {#add-int-int-int-int-java.io.InputStream-}
```
public int add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)
```


Adds a picture to the collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| leftColumn | int | Upper left column index. |
| bottomRow | int | Lower right row index |
| rightColumn | int | Lower right column index |
| stream | java.io.InputStream | Stream object which contains the image data. |

**Returns:**
int - [Picture](../../com.aspose.cells/picture) object index.
### add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName) {#add-int-int-int-int-java.lang.String-}
```
public int add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName)
```


Adds a picture to the collection.

**Example**

```
         //add a picture
         pictures.add(1, 1, 5, 5, "image.jpg");
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| leftColumn | int | Upper left column index. |
| bottomRow | int | Lower right row index |
| rightColumn | int | Lower right column index |
| fileName | java.lang.String | Image filename. |

**Returns:**
int - [Picture](../../com.aspose.cells/picture) object index.
### add(int topRow, int leftColumn, InputStream stream) {#add-int-int-java.io.InputStream-}
```
public int add(int topRow, int leftColumn, InputStream stream)
```


Adds a picture to the collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| leftColumn | int | Upper left column index. |
| stream | java.io.InputStream | Stream object which contains the image data. |

**Returns:**
int - [Picture](../../com.aspose.cells/picture) object index.
### add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale) {#add-int-int-java.io.InputStream-int-int-}
```
public int add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)
```


Adds a picture to the collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| leftColumn | int | Upper left column index. |
| stream | java.io.InputStream | Stream object which contains the image data. |
| widthScale | int | Scale of image width, a percentage. |
| heightScale | int | Scale of image height, a percentage. |

**Returns:**
int - [Picture](../../com.aspose.cells/picture) object index.
### add(int topRow, int leftColumn, String fileName) {#add-int-int-java.lang.String-}
```
public int add(int topRow, int leftColumn, String fileName)
```


Adds a picture to the collection.

**Example**

```
         //add a picture
         pictures.add(1, 1, "image.jpg");
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| leftColumn | int | Upper left column index. |
| fileName | java.lang.String | Image filename. |

**Returns:**
int - [Picture](../../com.aspose.cells/picture) object index.
### add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale) {#add-int-int-java.lang.String-int-int-}
```
public int add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale)
```


Adds a picture to the collection.

**Example**

```
         //add a picture
         pictures.add(1, 1, "image.jpg", 50, 50);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| leftColumn | int | Upper left column index. |
| fileName | java.lang.String | Image filename. |
| widthScale | int | Scale of image width, a percentage. |
| heightScale | int | Scale of image height, a percentage. |

**Returns:**
int - [Picture](../../com.aspose.cells/picture) object index.
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
### camera(int row, int column, String range) {#camera-int-int-java.lang.String-}
```
public int camera(int row, int column, String range)
```


Takes a photo of the range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index of this picture. |
| column | int | The column index of this picture. |
| range | java.lang.String | The area that requires photography |

**Returns:**
int - 
### clear() {#clear--}
```
public void clear()
```


Clear all pictures.

**Example**

```
         //clear
         pictures.clear();
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
public Picture get(int index)
```


Gets the [Picture](../../com.aspose.cells/picture) element at the specified index.

**Example**

```
         //get picture collection
         //PictureCollection pictures = workbook.Worksheets[0].Pictures;
         //add a picture
         int index = pictures.add(1, 1, "image.png");
         //get the picture
         Picture pic = pictures.get(index);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - The element at the specified index.
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


Remove shapes at the specific index

**Example**

```
         //add a picture
         int index2 = pictures.add(1, 1, "image.png");
         //delete
         pictures.removeAt(index2);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int |  |

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

