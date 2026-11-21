---
title: "ICellsDataTable"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar datatabell."
type: docs
url: /sv/java/com.aspose.cells/icellsdatatable/
---
```
public interface ICellsDataTable
```

Representerar datatabell.

**Remarks**
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [beforeFirst()](#beforeFirst--) | Flytta markören till början av detta objekt, precis före den första raden. |
| [get(int columnIndex)](#get-int-) | Hämtar data som lagras i kolumnen som anges av index. |
| [get(String columnName)](#get-java.lang.String-) | Hämtar data som lagras i kolumnen som anges av kolumnnamn. |
| [getColumns()](#getColumns--) | Hämtar kolumnernas namn. |
| [getCount()](#getCount--) | Hämtar antalet poster. -1 för okänt postantal. |
| [next()](#next--) | Flyttar markören ner en rad från dess nuvarande position. |
### beforeFirst() {#beforeFirst--}
```
public abstract void beforeFirst()
```


Flytta markören till början av detta objekt, precis före den första raden.

### get(int columnIndex) {#get-int-}
```
public abstract Object get(int columnIndex)
```


Hämtar data som lagras i kolumnen som anges av index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Den nollbaserade indexen för kolumnen. |

**Returns:**
java.lang.Object - 
### get(String columnName) {#get-java.lang.String-}
```
public abstract Object get(String columnName)
```


Hämtar data som lagras i kolumnen som anges av kolumnnamn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnName | java.lang.String | Kolumnnamnet. |

**Returns:**
java.lang.Object - 
### getColumns() {#getColumns--}
```
public abstract String[] getColumns()
```


Hämtar kolumnernas namn.

**Returns:**
java.lang.String[]
### getCount() {#getCount--}
```
public abstract int getCount()
```


Hämtar antalet poster. -1 för okänt postantal.

**Returns:**
int
### next() {#next--}
```
public abstract boolean next()
```


Flyttar markören ner en rad från dess nuvarande position.

**Returns:**
boolean - om den nya aktuella raden är giltig; false om det inte finns fler rader
