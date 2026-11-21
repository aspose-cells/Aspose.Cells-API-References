---
title: "PictureCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar en samling av objekt."
type: docs
url: /sv/java/com.aspose.cells/picturecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PictureCollection extends CollectionBase
```

Inkapslar en samling av [Picture](../../com.aspose.cells/picture)-objekt.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)](#add-int-int-int-int-java.io.InputStream-) | Lägger till en bild i samlingen. |
| [add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName)](#add-int-int-int-int-java.lang.String-) | Lägger till en bild i samlingen. |
| [add(int topRow, int leftColumn, InputStream stream)](#add-int-int-java.io.InputStream-) | Lägger till en bild i samlingen. |
| [add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)](#add-int-int-java.io.InputStream-int-int-) | Lägger till en bild i samlingen. |
| [add(int topRow, int leftColumn, String fileName)](#add-int-int-java.lang.String-) | Lägger till en bild i samlingen. |
| [add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale)](#add-int-int-java.lang.String-int-int-) | Lägger till en bild i samlingen. |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [camera(int row, int column, String range)](#camera-int-int-java.lang.String-) | Tar ett foto av området. |
| [clear()](#clear--) | Rensa alla bilder. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar [Picture](../../com.aspose.cells/picture)-elementet på det angivna indexet. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Ta bort former på det specifika indexet |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream) {#add-int-int-int-int-java.io.InputStream-}
```
public int add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)
```


Lägger till en bild i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| leftColumn | int | Övre vänstra kolumnindex. |
| bottomRow | int | Nedre högra radindex |
| rightColumn | int | Nedre högra kolumnindex |
| stream | java.io.InputStream | Strömobjekt som innehåller bilddata. |

**Returns:**
int – [Picture](../../com.aspose.cells/picture)-objektindex.
### add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName) {#add-int-int-int-int-java.lang.String-}
```
public int add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName)
```


Lägger till en bild i samlingen.

**Example**

```
         //add a picture
         pictures.add(1, 1, 5, 5, "image.jpg");
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| leftColumn | int | Övre vänstra kolumnindex. |
| bottomRow | int | Nedre högra radindex |
| rightColumn | int | Nedre högra kolumnindex |
| fileName | java.lang.String | Bildfilnamn. |

**Returns:**
int – [Picture](../../com.aspose.cells/picture)-objektindex.
### add(int topRow, int leftColumn, InputStream stream) {#add-int-int-java.io.InputStream-}
```
public int add(int topRow, int leftColumn, InputStream stream)
```


Lägger till en bild i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| leftColumn | int | Övre vänstra kolumnindex. |
| stream | java.io.InputStream | Strömobjekt som innehåller bilddata. |

**Returns:**
int – [Picture](../../com.aspose.cells/picture)-objektindex.
### add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale) {#add-int-int-java.io.InputStream-int-int-}
```
public int add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)
```


Lägger till en bild i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| leftColumn | int | Övre vänstra kolumnindex. |
| stream | java.io.InputStream | Strömobjekt som innehåller bilddata. |
| widthScale | int | Skala för bildens bredd, i procent. |
| heightScale | int | Skala för bildens höjd, i procent. |

**Returns:**
int – [Picture](../../com.aspose.cells/picture)-objektindex.
### add(int topRow, int leftColumn, String fileName) {#add-int-int-java.lang.String-}
```
public int add(int topRow, int leftColumn, String fileName)
```


Lägger till en bild i samlingen.

**Example**

```
         //add a picture
         pictures.add(1, 1, "image.jpg");
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| leftColumn | int | Övre vänstra kolumnindex. |
| fileName | java.lang.String | Bildfilnamn. |

**Returns:**
int – [Picture](../../com.aspose.cells/picture)-objektindex.
### add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale) {#add-int-int-java.lang.String-int-int-}
```
public int add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale)
```


Lägger till en bild i samlingen.

**Example**

```
         //add a picture
         pictures.add(1, 1, "image.jpg", 50, 50);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| leftColumn | int | Övre vänstra kolumnindex. |
| fileName | java.lang.String | Bildfilnamn. |
| widthScale | int | Skala för bildens bredd, i procent. |
| heightScale | int | Skala för bildens höjd, i procent. |

**Returns:**
int – [Picture](../../com.aspose.cells/picture)-objektindex.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Lägger till ett objekt i CollectionBase-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Objektet som ska läggas till i CollectionBase-instansen. |

**Returns:**
int - Positionen där det nya elementet infördes.
### camera(int row, int column, String range) {#camera-int-int-java.lang.String-}
```
public int camera(int row, int column, String range)
```


Tar ett foto av området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindexet för den här bilden. |
| kolumn | int | Kolumnindexet för den här bilden. |
| intervall | java.lang.String | Området som kräver fotografering |

**Returns:**
int -
### clear() {#clear--}
```
public void clear()
```


Rensa alla bilder.

**Example**

```
         //clear
         pictures.clear();
```

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Returnerar om instansen innehåller detta objekt

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | testobjekt |

**Returns:**
boolean - Om instansen innehåller detta objekt
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public Picture get(int index)
```


Hämtar [Picture](../../com.aspose.cells/picture)-elementet på det angivna indexet.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet. |

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


Hämtar antalet element som finns i CollectionBase-instansen.

**Returns:**
int - Antalet element som finns i CollectionBase-instansen.
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


Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |

**Returns:**
int - Indexet för värdet om det hittas i listan; annars -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Returnerar en enumerator som itererar genom CollectionBase-instansen.

**Returns:**
java.util.Iterator - En iterator för CollectionBase-instansen.
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


Ta bort former på det specifika indexet

**Example**

```
         //add a picture
         int index2 = pictures.add(1, 1, "image.png");
         //delete
         pictures.removeAt(index2);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

