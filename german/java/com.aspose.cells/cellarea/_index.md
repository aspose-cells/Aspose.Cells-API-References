---
title: "CellArea"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt einen Zellbereich dar."
type: docs
url: /de/java/com.aspose.cells/cellarea/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public final class CellArea implements Comparable
```

Stellt einen Zellbereich dar.

**Example**

```
         //Create Cell Area
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
```
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [CellArea()](#CellArea--) |  |
## Felder

| Feld | Beschreibung |
| --- | --- |
| [EndColumn](#EndColumn) | Liest oder setzt die Endspalte dieses Bereichs. |
| [EndRow](#EndRow) | Liest oder setzt die Endzeile dieses Bereichs. |
| [StartColumn](#StartColumn) | Liest oder setzt die Startspalte dieses Bereichs. |
| [StartRow](#StartRow) | Liest oder setzt die Startzeile dieses Bereichs. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [compareTo(Object obj)](#compareTo-java.lang.Object-) | Vergleicht zwei CellArea-Objekte anhand ihrer oberen linken Ecke. |
| [createCellArea(int startRow, int startColumn, int endRow, int endColumn)](#createCellArea-int-int-int-int-) | Erstellt einen Zellenbereich. |
| [createCellArea(String startCellName, String endCellName)](#createCellArea-java.lang.String-java.lang.String-) | Erstellt einen Zellenbereich. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | Gibt einen String zurück, der das aktuelle CellArea-Objekt darstellt. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CellArea() {#CellArea--}
```
public CellArea()
```


### EndColumn {#EndColumn}
```
public int EndColumn
```


Liest oder setzt die Endspalte dieses Bereichs.

### EndRow {#EndRow}
```
public int EndRow
```


Liest oder setzt die Endzeile dieses Bereichs.

### StartColumn {#StartColumn}
```
public int StartColumn
```


Liest oder setzt die Startspalte dieses Bereichs.

### StartRow {#StartRow}
```
public int StartRow
```


Liest oder setzt die Startzeile dieses Bereichs.

### compareTo(Object obj) {#compareTo-java.lang.Object-}
```
public int compareTo(Object obj)
```


Vergleicht zwei CellArea-Objekte anhand ihrer oberen linken Ecke.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
int - Wenn zwei Ecken in unterschiedlichen Zeilen liegen, wird ihr Zeilenindex verglichen. Andernfalls wird ihr Spaltenindex verglichen. Wenn beide Ecken gleich sind, wird 0 zurückgegeben.
### createCellArea(int startRow, int startColumn, int endRow, int endColumn) {#createCellArea-int-int-int-int-}
```
public static CellArea createCellArea(int startRow, int startColumn, int endRow, int endColumn)
```


Erstellt einen Zellenbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Die Startzeile. |
| startColumn | int | Die Startspalte. |
| endRow | int | Die Endzeile. |
| endColumn | int | Die Endspalte. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Return a [CellArea](../../com.aspose.cells/cellarea).
### createCellArea(String startCellName, String endCellName) {#createCellArea-java.lang.String-java.lang.String-}
```
public static CellArea createCellArea(String startCellName, String endCellName)
```


Erstellt einen Zellenbereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startCellName | java.lang.String | Die obere linke Zelle des Bereichs. |
| endCellName | java.lang.String | Die untere rechte Zelle des Bereichs. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Return a [CellArea](../../com.aspose.cells/cellarea).
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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




### toString() {#toString--}
```
public String toString()
```


Gibt einen String zurück, der das aktuelle CellArea-Objekt darstellt.

**Returns:**
java.lang.String -
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

