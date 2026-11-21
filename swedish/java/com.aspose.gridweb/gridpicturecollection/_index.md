---
title: "GridPictureCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar en samling av objekt."
type: docs
url: /sv/java/com.aspose.gridweb/gridpicturecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridPictureCollection
```

Innesluter en samling av [GridPicture](../../com.aspose.gridweb/gridpicture) objekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, String fileName)](#add-int-int-int-int-java.lang.String-) | Lägger till en bild i samlingen. |
| [add(int upperLeftRow, int upperLeftColumn, String fileName)](#add-int-int-java.lang.String-) | Lägger till en bild i samlingen. |
| [add(int upperLeftRow, int upperLeftColumn, String fileName, int widthScale, int heightScale)](#add-int-int-java.lang.String-int-int-) | Lägger till en bild i samlingen. |
| [clear()](#clear--) | Rensa alla bilder. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar [GridPicture](../../com.aspose.gridweb/gridpicture)-elementet på det angivna indexet. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar storleken på enumeratorn |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Hämtar enumerator för rader |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int param_int)](#removeAt-int-) | Ta bort former på det specifika indexet |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, String fileName) {#add-int-int-int-int-java.lang.String-}
```
public int add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, String fileName)
```


Lägger till en bild i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| upperLeftRow | int | Övre vänstra radindex. |
| upperLeftColumn | int | Övre vänstra kolumnindex. |
| lowerRightRow | int | Nedre högra radindex |
| lowerRightColumn | int | Nedre högra kolumnindex |
| fileName | java.lang.String | Bildfilnamn. |

**Returns:**
int - [GridPicture](../../com.aspose.gridweb/gridpicture) objektindex.
### add(int upperLeftRow, int upperLeftColumn, String fileName) {#add-int-int-java.lang.String-}
```
public int add(int upperLeftRow, int upperLeftColumn, String fileName)
```


Lägger till en bild i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| upperLeftRow | int | Övre vänstra radindex. |
| upperLeftColumn | int | Övre vänstra kolumnindex. |
| fileName | java.lang.String | Bildfilnamn. |

**Returns:**
int - [GridPicture](../../com.aspose.gridweb/gridpicture) objektindex.
### add(int upperLeftRow, int upperLeftColumn, String fileName, int widthScale, int heightScale) {#add-int-int-java.lang.String-int-int-}
```
public int add(int upperLeftRow, int upperLeftColumn, String fileName, int widthScale, int heightScale)
```


Lägger till en bild i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| upperLeftRow | int | Övre vänstra radindex. |
| upperLeftColumn | int | Övre vänstra kolumnindex. |
| fileName | java.lang.String | Bildfilnamn. |
| widthScale | int | Skala för bildens bredd, i procent. |
| heightScale | int | Skala för bildens höjd, i procent. |

**Returns:**
int - [GridPicture](../../com.aspose.gridweb/gridpicture) objektindex.
### clear() {#clear--}
```
public void clear()
```


Rensa alla bilder.

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
public GridPicture get(int index)
```


Hämtar [GridPicture](../../com.aspose.gridweb/gridpicture)-elementet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet. |

**Returns:**
[GridPicture](../../com.aspose.gridweb/gridpicture) - The element at the specified index.
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


Hämtar storleken på enumeratorn

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


Hämtar enumerator för rader

**Returns:**
java.util.Iterator - Enumeratör för rader
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int param_int) {#removeAt-int-}
```
public void removeAt(int param_int)
```


Ta bort former på det specifika indexet

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| param_int | int |  |

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

