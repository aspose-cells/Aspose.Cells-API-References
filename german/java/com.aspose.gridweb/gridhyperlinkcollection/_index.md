---
title: "GridHyperlinkCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt eine Sammlung von Objekten."
type: docs
url: /de/java/com.aspose.gridweb/gridhyperlinkcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridHyperlinkCollection
```

Kapselt eine Sammlung von [GridHyperlink](../../com.aspose.gridweb/gridhyperlink)-Objekten.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)](#add-int-int-int-int-java.lang.String-) | Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu. |
| [add(String cellName, int totalRows, int totalColumns, String address)](#add-java.lang.String-int-int-java.lang.String-) | Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu. |
| [add(String cellName, String address)](#add-java.lang.String-java.lang.String-) | Fügt einem angegebenen Feld einen Hyperlink hinzu. |
| [add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)](#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu. |
| [clear()](#clear--) | Löscht alle Hyperlinks. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Liefert das [GridHyperlink](../../com.aspose.gridweb/gridhyperlink)-Element am angegebenen Index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ruft die Größe des Enumerators ab. |
| [getHyperlink(GridCell cell)](#getHyperlink-com.aspose.gridweb.GridCell-) | Liefert das Hyperlink-Objekt der Zelle. |
| [getHyperlink(int row, int column)](#getHyperlink-int-int-) | Liefert das Hyperlink-Objekt der Zelle. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(GridCellArea area)](#remove-com.aspose.gridweb.GridCellArea-) | Entfernt den Hyperlink im angegebenen Bereich. |
| [removeAt(int index)](#removeAt-int-) | Entfernt den Hyperlink am angegebenen Index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address) {#add-int-int-int-int-java.lang.String-}
```
public int add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)
```


Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | int | Erste Zeile des Hyperlink-Bereichs. |
| firstColumn | int | Erste Spalte des Hyperlink-Bereichs. |
| totalRows | int | Anzahl der Zeilen in diesem Hyperlink-Bereich. |
| totalColumns | int | Anzahl der Spalten dieses Hyperlink-Bereichs. |
| Adresse | java.lang.String | Adresse des Hyperlinks. |

**Returns:**
int - Index des [GridHyperlink](../../com.aspose.gridweb/gridhyperlink)-Objekts.
### add(String cellName, int totalRows, int totalColumns, String address) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String cellName, int totalRows, int totalColumns, String address)
```


Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Zellenname. |
| totalRows | int | Anzahl der Zeilen in diesem Hyperlink-Bereich. |
| totalColumns | int | Anzahl der Spalten dieses Hyperlink-Bereichs. |
| Adresse | java.lang.String | Adresse des Hyperlinks. |

**Returns:**
int - Index des [GridHyperlink](../../com.aspose.gridweb/gridhyperlink)-Objekts.
### add(String cellName, String address) {#add-java.lang.String-java.lang.String-}
```
public int add(String cellName, String address)
```


Fügt einem angegebenen Feld einen Hyperlink hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Zellenname. |
| Adresse | java.lang.String | Adresse des Hyperlinks. |

**Returns:**
int - Index des [GridHyperlink](../../com.aspose.gridweb/gridhyperlink)-Objekts.
### add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip) {#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)
```


Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startCellName | java.lang.String | Die obere linke Zelle des Bereichs. |
| endCellName | java.lang.String | Die untere rechte Zelle des Bereichs. |
| Adresse | java.lang.String | Adresse des Hyperlinks. |
| textToDisplay | java.lang.String | Der Text, der für den angegebenen Hyperlink angezeigt wird. |
| screenTip | java.lang.String | Der ScreenTip-Text für den angegebenen Hyperlink. |

**Returns:**
int - Index des [GridHyperlink](../../com.aspose.gridweb/gridhyperlink)-Objekts.
### clear() {#clear--}
```
public void clear()
```


Löscht alle Hyperlinks.

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
public GridHyperlink get(int index)
```


Liefert das [GridHyperlink](../../com.aspose.gridweb/gridhyperlink)-Element am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des Elements. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - The element at the specified index.
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
### getHyperlink(GridCell cell) {#getHyperlink-com.aspose.gridweb.GridCell-}
```
public GridHyperlink getHyperlink(GridCell cell)
```


Liefert das Hyperlink-Objekt der Zelle. Wenn die Zelle keinen Hyperlink hat, wird null zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cell | [GridCell](../../com.aspose.gridweb/gridcell) | Das GridCell-Objekt. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) the GridHyperlink object.
### getHyperlink(int row, int column) {#getHyperlink-int-int-}
```
public GridHyperlink getHyperlink(int row, int column)
```


Liefert das Hyperlink-Objekt der Zelle. Wenn die Zelle keinen Hyperlink hat, wird null zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Die Zeile der Zelle. |
| Spalte | int | Die Spalte der Zelle. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) the GridHyperlink object.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(GridCellArea area) {#remove-com.aspose.gridweb.GridCellArea-}
```
public void remove(GridCellArea area)
```


Entfernt den Hyperlink im angegebenen Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Der Bereich, der den Hyperlink enthält. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Entfernt den Hyperlink am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des Elements. |

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

