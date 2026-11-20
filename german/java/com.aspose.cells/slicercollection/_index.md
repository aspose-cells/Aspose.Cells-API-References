---
title: "SlicerCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Gibt die Sammlung aller Slicer-Objekte im angegebenen Arbeitsblatt an."
type: docs
url: /de/java/com.aspose.cells/slicercollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SlicerCollection extends CollectionBase
```

Gibt die Sammlung aller Slicer-Objekte im angegebenen Arbeitsblatt an.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
 
         SlicerCollection slicers = sheet.getSlicers();
         int slicerIndex = slicers.add(pivot, "E12", "fruit");
         Slicer slicer = slicers.get(slicerIndex);
 
         //do your business
 
         book.save("out.xlsx");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(ListObject table, ListColumn listColumn, int row, int column)](#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-int-int-) | Fügt einen neuen Slicer hinzu, der ListObjet als Datenquelle verwendet |
| [add(ListObject table, ListColumn listColumn, String destCellName)](#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-java.lang.String-) | Fügt einen neuen Slicer hinzu, der ListObjet als Datenquelle verwendet |
| [add(ListObject table, int index, String destCellName)](#add-com.aspose.cells.ListObject-int-java.lang.String-) | Fügt einen neuen Slicer hinzu, der ListObjet als Datenquelle verwendet |
| [add(PivotTable pivot, int row, int column, PivotField baseField)](#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-) | Fügt einen neuen Slicer hinzu, der PivotTable als Datenquelle verwendet |
| [add(PivotTable pivot, int row, int column, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-int-int-int-) | Fügt einen neuen Slicer hinzu, der PivotTable als Datenquelle verwendet |
| [add(PivotTable pivot, int row, int column, String baseFieldName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | Fügt einen neuen Slicer hinzu, der PivotTable als Datenquelle verwendet |
| [add(PivotTable pivot, String destCellName, PivotField baseField)](#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-) | Fügt einen neuen Slicer hinzu, der PivotTable als Datenquelle verwendet |
| [add(PivotTable pivot, String destCellName, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-java.lang.String-int-) | Fügt einen neuen Slicer hinzu, der PivotTable als Datenquelle verwendet |
| [add(PivotTable pivot, String destCellName, String baseFieldName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | Fügt einen neuen Slicer hinzu, der PivotTable als Datenquelle verwendet |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [clear()](#clear--) | Alle Slicer löschen. |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ruft den Slicer nach Index ab. |
| [get(String name)](#get-java.lang.String-) | Ruft den Slicer nach Namen des Slicers ab. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Slicer slicer)](#remove-com.aspose.cells.Slicer-) | Entfernt den angegebenen Slicer |
| [removeAt(int index)](#removeAt-int-) | Löscht den Slicer am angegebenen Index |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(ListObject table, ListColumn listColumn, int row, int column) {#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-int-int-}
```
public int add(ListObject table, ListColumn listColumn, int row, int column)
```


Fügt einen neuen Slicer hinzu, der ListObjet als Datenquelle verwendet

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject-Objekt |
| listColumn | [ListColumn](../../com.aspose.cells/listcolumn) | Die ListColumn in ListObject.ListColumns |
| Zeile | int | Zeilenindex der Zelle in der oberen linken Ecke des Slicer‑Bereichs. |
| Spalte | int | Spaltenindex der Zelle in der oberen linken Ecke des Slicer‑Bereichs. |

**Returns:**
int – Der neue hinzugefügte Slicer‑Index
### add(ListObject table, ListColumn listColumn, String destCellName) {#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-java.lang.String-}
```
public int add(ListObject table, ListColumn listColumn, String destCellName)
```


Fügt einen neuen Slicer hinzu, der ListObjet als Datenquelle verwendet

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject-Objekt |
| listColumn | [ListColumn](../../com.aspose.cells/listcolumn) | Die ListColumn in ListObject.ListColumns |
| destCellName | java.lang.String | Die Zelle in der oberen linken Ecke des Slicer‑Bereichs. |

**Returns:**
int – Der neue hinzugefügte Slicer‑Index
### add(ListObject table, int index, String destCellName) {#add-com.aspose.cells.ListObject-int-java.lang.String-}
```
public int add(ListObject table, int index, String destCellName)
```


Fügt einen neuen Slicer hinzu, der ListObjet als Datenquelle verwendet

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject-Objekt |
| Index | int | Der Index der ListColumn in ListObject.ListColumns |
| destCellName | java.lang.String | Die Zelle in der oberen linken Ecke des Slicer‑Bereichs. |

**Returns:**
int – Der neue hinzugefügte Slicer‑Index
### add(PivotTable pivot, int row, int column, PivotField baseField) {#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, int row, int column, PivotField baseField)
```


Fügt einen neuen Slicer hinzu, der PivotTable als Datenquelle verwendet

**Example**

```
         slicers.add(pivot, 3, 12, pivot.getBaseFields().get(0));
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-Objekt |
| Zeile | int | Zeilenindex der Zelle in der oberen linken Ecke des Slicer‑Bereichs. |
| Spalte | int | Spaltenindex der Zelle in der oberen linken Ecke des Slicer‑Bereichs. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | Das PivotField in PivotTable.BaseFields |

**Returns:**
int – Der neue hinzugefügte Slicer‑Index
### add(PivotTable pivot, int row, int column, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-int-int-int-}
```
public int add(PivotTable pivot, int row, int column, int baseFieldIndex)
```


Fügt einen neuen Slicer hinzu, der PivotTable als Datenquelle verwendet

**Example**

```
         slicers.add(pivot, 20, 8, 0);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-Objekt |
| Zeile | int | Zeilenindex der Zelle in der oberen linken Ecke des Slicer‑Bereichs. |
| Spalte | int | Spaltenindex der Zelle in der oberen linken Ecke des Slicer‑Bereichs. |
| baseFieldIndex | int | Der Index des PivotField in PivotTable.BaseFields |

**Returns:**
int – Der neue hinzugefügte Slicer‑Index
### add(PivotTable pivot, int row, int column, String baseFieldName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivot, int row, int column, String baseFieldName)
```


Fügt einen neuen Slicer hinzu, der PivotTable als Datenquelle verwendet

**Example**

```
         slicers.add(pivot, 20, 12, "fruit");
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-Objekt |
| Zeile | int | Zeilenindex der Zelle in der oberen linken Ecke des Slicer‑Bereichs. |
| Spalte | int | Spaltenindex der Zelle in der oberen linken Ecke des Slicer‑Bereichs. |
| baseFieldName | java.lang.String | Der Name des PivotField in PivotTable.BaseFields |

**Returns:**
int – Der neue hinzugefügte Slicer‑Index
### add(PivotTable pivot, String destCellName, PivotField baseField) {#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, String destCellName, PivotField baseField)
```


Fügt einen neuen Slicer hinzu, der PivotTable als Datenquelle verwendet

**Example**

```
         slicers.add(pivot, "I3", pivot.getBaseFields().get(0));
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-Objekt |
| destCellName | java.lang.String | Die Zelle in der oberen linken Ecke des Slicer‑Bereichs. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | Das PivotField in PivotTable.BaseFields |

**Returns:**
int – Der neue hinzugefügte Slicer‑Index
### add(PivotTable pivot, String destCellName, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-java.lang.String-int-}
```
public int add(PivotTable pivot, String destCellName, int baseFieldIndex)
```


Fügt einen neuen Slicer hinzu, der PivotTable als Datenquelle verwendet

**Example**

```
         slicers.add(pivot, "E20", 0);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-Objekt |
| destCellName | java.lang.String | Die Zelle in der oberen linken Ecke des Slicer‑Bereichs. |
| baseFieldIndex | int | Der Index des PivotField in PivotTable.BaseFields |

**Returns:**
int – Der neue hinzugefügte Slicer‑Index
### add(PivotTable pivot, String destCellName, String baseFieldName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivot, String destCellName, String baseFieldName)
```


Fügt einen neuen Slicer hinzu, der PivotTable als Datenquelle verwendet

**Example**

```
         slicers.add(pivot, "E3", "fruit");
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-Objekt |
| destCellName | java.lang.String | Die Zelle in der oberen linken Ecke des Slicer‑Bereichs. |
| baseFieldName | java.lang.String | Der Name des PivotField in PivotTable.BaseFields |

**Returns:**
int – Der neue hinzugefügte Slicer‑Index
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Fügt ein Element zur CollectionBase-Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Das Objekt, das zur CollectionBase-Instanz hinzugefügt werden soll. |

**Returns:**
int - Die Position, an der das neue Element eingefügt wurde.
### clear() {#clear--}
```
public void clear()
```


Alle Slicer löschen.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Gibt zurück, ob die Instanz dieses Objekt enthält

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Testobjekt |

**Returns:**
boolean - Ob die Instanz dieses Objekt enthält
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
public Slicer get(int index)
```


Ruft den Slicer nach Index ab.

**Example**

```
         Slicer slicerByIndex = slicers.get(0);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int |  |

**Returns:**
[Slicer](../../com.aspose.cells/slicer)
### get(String name) {#get-java.lang.String-}
```
public Slicer get(String name)
```


Ruft den Slicer nach Namen des Slicers ab.

**Example**

```
         Slicer slicerByName = slicers.get("fruit");
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[Slicer](../../com.aspose.cells/slicer)
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


Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.

**Returns:**
int - Die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.
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


Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |

**Returns:**
int - Der Index des Wertes, falls in der Liste gefunden; sonst -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft.

**Returns:**
java.util.Iterator - Ein Iterator für die CollectionBase-Instanz.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(Slicer slicer) {#remove-com.aspose.cells.Slicer-}
```
public void remove(Slicer slicer)
```


Entfernt den angegebenen Slicer

**Example**

```
         Slicer delSlicer = slicers.get(0);
         slicers.remove(delSlicer);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| slicer | [Slicer](../../com.aspose.cells/slicer) | Das Slicer-Objekt |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Löscht den Slicer am angegebenen Index

**Example**

```
         slicers.removeAt(1);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Positionsindex in der Slicer-Sammlung |

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

