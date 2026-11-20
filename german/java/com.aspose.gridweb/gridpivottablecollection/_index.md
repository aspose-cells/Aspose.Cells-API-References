---
title: "GridPivotTableCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt eine Sammlung von Objekten."
type: docs
url: /de/java/com.aspose.gridweb/gridpivottablecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridPivotTableCollection
```

Kapselt eine Sammlung von [GridPivotTable](../../com.aspose.gridweb/gridpivottable) Objekten.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName)](#add-com.aspose.gridweb.GridWorksheet-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-) | Fügt einen neuen PivotTable-Cache zu einer PivotCaches-Sammlung hinzu. |
| [add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName)](#add-java.lang.String-com.aspose.gridweb.GridCellArea-int-int-java.lang.String-) | Fügt einen neuen PivotTable-Cache zu einer PivotCaches-Sammlung hinzu. |
| [add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName)](#add-java.lang.String-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-) | Fügt einen neuen PivotTable-Cache zu einer PivotCaches-Sammlung hinzu. |
| [add(String sourceData, String destCellName, String tableName)](#add-java.lang.String-java.lang.String-java.lang.String-) | Fügt einen neuen PivotTable-Cache zu einer PivotCaches-Sammlung hinzu. |
| [clear()](#clear--) | Löscht alle PivotTables. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ruft das [GridPivotTable](../../com.aspose.gridweb/gridpivottable) Element am angegebenen Index ab. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ruft die Größe des Enumerators ab. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Entfernt die PivotTable am angegebenen Index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName) {#add-com.aspose.gridweb.GridWorksheet-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-}
```
public int add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName)
```


Fügt einen neuen PivotTable-Cache zu einer PivotCaches-Sammlung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceSheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | Das Quell-Arbeitsblatt. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Der Bereich im Quell-Arbeitsblatt. |
| destCellName | java.lang.String | Die Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | java.lang.String | Der Name des neuen PivotTable-Berichts. |

**Returns:**
int - Der neu hinzugefügte Cache-Index.
### add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName) {#add-java.lang.String-com.aspose.gridweb.GridCellArea-int-int-java.lang.String-}
```
public int add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName)
```


Fügt einen neuen PivotTable-Cache zu einer PivotCaches-Sammlung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| worksheetname | java.lang.String | Der Name des Quell-Arbeitsblatts. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Der Bereich im Quell-Arbeitsblatt. |
| destRow | int | Die Zeile der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| destCol | int | Die Spalte der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | java.lang.String | Der Name des neuen PivotTable-Berichts. |

**Returns:**
int - Der neu hinzugefügte Cache-Index.
### add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName) {#add-java.lang.String-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-}
```
public int add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName)
```


Fügt einen neuen PivotTable-Cache zu einer PivotCaches-Sammlung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| worksheetname | java.lang.String | Der Name des Quell-Arbeitsblatts. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Der Bereich im Quell-Arbeitsblatt. |
| destCellName | java.lang.String | Die Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | java.lang.String | Der Name des neuen PivotTable-Berichts. |

**Returns:**
int - Der neu hinzugefügte Cache-Index.
### add(String sourceData, String destCellName, String tableName) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String sourceData, String destCellName, String tableName)
```


Fügt einen neuen PivotTable-Cache zu einer PivotCaches-Sammlung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | java.lang.String | Der Datenzellenbereich für die neue PivotTable. Beispiel: Sheet1!A1:C8 |
| destCellName | java.lang.String | Die Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | java.lang.String | Der Name des neuen PivotTable-Berichts. |

**Returns:**
int - Der neu hinzugefügte Cache-Index.
### clear() {#clear--}
```
public void clear()
```


Löscht alle PivotTables.

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
public GridPivotTable get(int index)
```


Ruft das [GridPivotTable](../../com.aspose.gridweb/gridpivottable) Element am angegebenen Index ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des Elements. |

**Returns:**
[GridPivotTable](../../com.aspose.gridweb/gridpivottable) - The element at the specified index.
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


Entfernt die PivotTable am angegebenen Index.

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

