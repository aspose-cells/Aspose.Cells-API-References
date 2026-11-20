---
title: "GridPictureCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt eine Sammlung von Objekten."
type: docs
url: /de/java/com.aspose.gridweb/gridpicturecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridPictureCollection
```

Kapselt eine Sammlung von [GridPicture](../../com.aspose.gridweb/gridpicture)-Objekten.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, String fileName)](#add-int-int-int-int-java.lang.String-) | Fügt ein Bild zur Sammlung hinzu. |
| [add(int upperLeftRow, int upperLeftColumn, String fileName)](#add-int-int-java.lang.String-) | Fügt ein Bild zur Sammlung hinzu. |
| [add(int upperLeftRow, int upperLeftColumn, String fileName, int widthScale, int heightScale)](#add-int-int-java.lang.String-int-int-) | Fügt ein Bild zur Sammlung hinzu. |
| [clear()](#clear--) | Alle Bilder löschen. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Liefert das [GridPicture](../../com.aspose.gridweb/gridpicture)-Element am angegebenen Index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ruft die Größe des Enumerators ab. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Ruft den Zeilen-Enumerator ab. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int param_int)](#removeAt-int-) | Formen am angegebenen Index entfernen |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, String fileName) {#add-int-int-int-int-java.lang.String-}
```
public int add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, String fileName)
```


Fügt ein Bild zur Sammlung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| upperLeftRow | int | Index der oberen linken Zeile. |
| upperLeftColumn | int | Index der oberen linken Spalte. |
| lowerRightRow | int | Index der unteren rechten Zeile |
| lowerRightColumn | int | Index der unteren rechten Spalte |
| fileName | java.lang.String | Bilddateiname. |

**Returns:**
int – Index des [GridPicture](../../com.aspose.gridweb/gridpicture)-Objekts.
### add(int upperLeftRow, int upperLeftColumn, String fileName) {#add-int-int-java.lang.String-}
```
public int add(int upperLeftRow, int upperLeftColumn, String fileName)
```


Fügt ein Bild zur Sammlung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| upperLeftRow | int | Index der oberen linken Zeile. |
| upperLeftColumn | int | Index der oberen linken Spalte. |
| fileName | java.lang.String | Bilddateiname. |

**Returns:**
int – Index des [GridPicture](../../com.aspose.gridweb/gridpicture)-Objekts.
### add(int upperLeftRow, int upperLeftColumn, String fileName, int widthScale, int heightScale) {#add-int-int-java.lang.String-int-int-}
```
public int add(int upperLeftRow, int upperLeftColumn, String fileName, int widthScale, int heightScale)
```


Fügt ein Bild zur Sammlung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| upperLeftRow | int | Index der oberen linken Zeile. |
| upperLeftColumn | int | Index der oberen linken Spalte. |
| fileName | java.lang.String | Bilddateiname. |
| widthScale | int | Skalierung der Bildbreite, ein Prozentsatz. |
| heightScale | int | Skalierung der Bildhöhe, ein Prozentsatz. |

**Returns:**
int – Index des [GridPicture](../../com.aspose.gridweb/gridpicture)-Objekts.
### clear() {#clear--}
```
public void clear()
```


Alle Bilder löschen.

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
public GridPicture get(int index)
```


Liefert das [GridPicture](../../com.aspose.gridweb/gridpicture)-Element am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des Elements. |

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




### removeAt(int param_int) {#removeAt-int-}
```
public void removeAt(int param_int)
```


Formen am angegebenen Index entfernen

**Parameters:**
| Parameter | Typ | Beschreibung |
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

