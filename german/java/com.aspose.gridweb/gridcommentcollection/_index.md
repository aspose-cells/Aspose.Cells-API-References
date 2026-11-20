---
title: "GridCommentCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt eine Sammlung von Objekten."
type: docs
url: /de/java/com.aspose.gridweb/gridcommentcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridCommentCollection
```

Kapselt eine Sammlung von [GridComment](../../com.aspose.gridweb/gridcomment)-Objekten.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(int row, int column)](#add-int-int-) | Fügt der Sammlung einen Kommentar hinzu. |
| [add(String cellName)](#add-java.lang.String-) | Fügt der Sammlung einen Kommentar hinzu. |
| [clear()](#clear--) | Entfernt alle Kommentare; |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Liefert das [GridComment](../../com.aspose.gridweb/gridcomment)-Element am angegebenen Index. |
| [get(int row, int column)](#get-int-int-) | Liefert das [GridComment](../../com.aspose.gridweb/gridcomment)-Element am angegebenen Zeilenindex und Spaltenindex. |
| [get(String cellName)](#get-java.lang.String-) | Ruft das [GridComment](../../com.aspose.gridweb/gridcomment)-Element an der angegebenen Zelle ab. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ruft die Größe des Enumerators ab. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Ruft den Zeilen-Enumerator ab. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int row, int column)](#removeAt-int-int-) | Entfernt den Kommentar der angegebenen Zelle. |
| [removeAt(String cellName)](#removeAt-java.lang.String-) | Entfernt den Kommentar der angegebenen Zelle. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


Fügt der Sammlung einen Kommentar hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex der Zelle. |
| Spalte | int | Spaltenindex der Zelle. |

**Returns:**
int – [GridComment](../../com.aspose.gridweb/gridcomment)-Objektindex.
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```


Fügt der Sammlung einen Kommentar hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Zellenname. |

**Returns:**
int – [GridComment](../../com.aspose.gridweb/gridcomment)-Objektindex.
### clear() {#clear--}
```
public void clear()
```


Entfernt alle Kommentare;

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public GridComment get(int index)
```


Liefert das [GridComment](../../com.aspose.gridweb/gridcomment)-Element am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des Elements. |

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - The element at the specified index.
### get(int row, int column) {#get-int-int-}
```
public GridComment get(int row, int column)
```


Liefert das [GridComment](../../com.aspose.gridweb/gridcomment)-Element am angegebenen Zeilenindex und Spaltenindex.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |
| Spalte | int | Spaltenindex. |

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - The element at the specified cell.
### get(String cellName) {#get-java.lang.String-}
```
public GridComment get(String cellName)
```


Ruft das [GridComment](../../com.aspose.gridweb/gridcomment)-Element an der angegebenen Zelle ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Zellenname. |

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


Ruft die Größe des Enumerators ab.

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


Ruft den Zeilen-Enumerator ab.

**Returns:**
java.util.Iterator – Der Zeilen-Enumerator.
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


Entfernt den Kommentar der angegebenen Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Der Zeilenindex. |
| Spalte | int | der Spaltenindex. |

### removeAt(String cellName) {#removeAt-java.lang.String-}
```
public void removeAt(String cellName)
```


Entfernt den Kommentar der angegebenen Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Der Name der Zelle, die einen Kommentar enthält. |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

