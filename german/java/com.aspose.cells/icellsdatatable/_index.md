---
title: "ICellsDataTable"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt eine Datentabelle dar."
type: docs
url: /de/java/com.aspose.cells/icellsdatatable/
---
```
public interface ICellsDataTable
```

Stellt eine Datentabelle dar.

**Remarks**
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [beforeFirst()](#beforeFirst--) | Bewegen Sie den Cursor an den Anfang dieses Objekts, direkt vor die erste Zeile. |
| [get(int columnIndex)](#get-int-) | Liest die in der durch den Index angegebenen Spalte gespeicherten Daten. |
| [get(String columnName)](#get-java.lang.String-) | Liest die in der durch den Spaltennamen angegebenen Spalte gespeicherten Daten. |
| [getColumns()](#getColumns--) | Liest den Namen der Spalten. |
| [getCount()](#getCount--) | Liest die Anzahl der Datensätze. -1 für unbekannte Datensatzanzahl. |
| [next()](#next--) | Bewegt den Cursor eine Zeile nach unten von seiner aktuellen Position. |
### beforeFirst() {#beforeFirst--}
```
public abstract void beforeFirst()
```


Bewegen Sie den Cursor an den Anfang dieses Objekts, direkt vor die erste Zeile.

### get(int columnIndex) {#get-int-}
```
public abstract Object get(int columnIndex)
```


Liest die in der durch den Index angegebenen Spalte gespeicherten Daten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Der nullbasierte Index der Spalte. |

**Returns:**
java.lang.Object -
### get(String columnName) {#get-java.lang.String-}
```
public abstract Object get(String columnName)
```


Liest die in der durch den Spaltennamen angegebenen Spalte gespeicherten Daten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnName | java.lang.String | Der Spaltenname. |

**Returns:**
java.lang.Object -
### getColumns() {#getColumns--}
```
public abstract String[] getColumns()
```


Liest den Namen der Spalten.

**Returns:**
java.lang.String[]
### getCount() {#getCount--}
```
public abstract int getCount()
```


Liest die Anzahl der Datensätze. -1 für unbekannte Datensatzanzahl.

**Returns:**
int
### next() {#next--}
```
public abstract boolean next()
```


Bewegt den Cursor eine Zeile nach unten von seiner aktuellen Position.

**Returns:**
boolean - wenn die neue aktuelle Zeile gültig ist; false, wenn keine weiteren Zeilen mehr vorhanden sind
