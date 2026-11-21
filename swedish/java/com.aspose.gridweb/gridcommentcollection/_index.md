---
title: "GridCommentCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar en samling av objekt."
type: docs
url: /sv/java/com.aspose.gridweb/gridcommentcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridCommentCollection
```

Inkapslar en samling av [GridComment](../../com.aspose.gridweb/gridcomment) objekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(int row, int column)](#add-int-int-) | Lägger till en kommentar i samlingen. |
| [add(String cellName)](#add-java.lang.String-) | Lägger till en kommentar i samlingen. |
| [clear()](#clear--) | Tar bort alla kommentarer; |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar [GridComment](../../com.aspose.gridweb/gridcomment) elementet på det angivna indexet. |
| [get(int row, int column)](#get-int-int-) | Hämtar [GridComment](../../com.aspose.gridweb/gridcomment) elementet på det angivna radindexet och kolumnindexet. |
| [get(String cellName)](#get-java.lang.String-) | Hämtar [GridComment](../../com.aspose.gridweb/gridcomment) elementet på den angivna cellen. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar storleken på enumeratorn |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Hämtar enumerator för rader |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int row, int column)](#removeAt-int-int-) | Tar bort kommentaren för den specifika cellen. |
| [removeAt(String cellName)](#removeAt-java.lang.String-) | Tar bort kommentaren för den specifika cellen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


Lägger till en kommentar i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Cellens radindex. |
| kolumn | int | Cellens kolumnindex. |

**Returns:**
int - [GridComment](../../com.aspose.gridweb/gridcomment) objektindex.
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```


Lägger till en kommentar i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellNamn | java.lang.String | Cellnamn. |

**Returns:**
int - [GridComment](../../com.aspose.gridweb/gridcomment) objektindex.
### clear() {#clear--}
```
public void clear()
```


Tar bort alla kommentarer;

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
public GridComment get(int index)
```


Hämtar [GridComment](../../com.aspose.gridweb/gridcomment) elementet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet. |

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - The element at the specified index.
### get(int row, int column) {#get-int-int-}
```
public GridComment get(int row, int column)
```


Hämtar [GridComment](../../com.aspose.gridweb/gridcomment) elementet på det angivna radindexet och kolumnindexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |
| kolumn | int | Kolumnindex. |

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - The element at the specified cell.
### get(String cellName) {#get-java.lang.String-}
```
public GridComment get(String cellName)
```


Hämtar [GridComment](../../com.aspose.gridweb/gridcomment) elementet på den angivna cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellNamn | java.lang.String | Cellnamn. |

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - The element at the specified cell.
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




### removeAt(int row, int column) {#removeAt-int-int-}
```
public void removeAt(int row, int column)
```


Tar bort kommentaren för den specifika cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindexet. |
| kolumn | int | kolumnens index. |

### removeAt(String cellName) {#removeAt-java.lang.String-}
```
public void removeAt(String cellName)
```


Tar bort kommentaren för den specifika cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellNamn | java.lang.String | Namnet på cellen som innehåller en kommentar. |

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

