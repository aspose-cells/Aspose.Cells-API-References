---
title: "ICellsDataTable"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta la tabella dei dati."
type: docs
url: /it/java/com.aspose.cells/icellsdatatable/
---
```
public interface ICellsDataTable
```

Rappresenta la tabella dei dati.

**Remarks**
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [beforeFirst()](#beforeFirst--) | Sposta il cursore all'inizio di questo oggetto, appena prima della prima riga. |
| [get(int columnIndex)](#get-int-) | Ottiene i dati memorizzati nella colonna specificata per indice. |
| [get(String columnName)](#get-java.lang.String-) | Ottiene i dati memorizzati nella colonna specificata per nome della colonna. |
| [getColumns()](#getColumns--) | Ottiene il nome delle colonne. |
| [getCount()](#getCount--) | Ottiene il conteggio dei record. -1 per conteggio dei record sconosciuto. |
| [next()](#next--) | Sposta il cursore di una riga verso il basso dalla sua posizione attuale. |
### beforeFirst() {#beforeFirst--}
```
public abstract void beforeFirst()
```


Sposta il cursore all'inizio di questo oggetto, appena prima della prima riga.

### get(int columnIndex) {#get-int-}
```
public abstract Object get(int columnIndex)
```


Ottiene i dati memorizzati nella colonna specificata per indice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | L'indice della colonna basato su zero. |

**Returns:**
java.lang.Object -
### get(String columnName) {#get-java.lang.String-}
```
public abstract Object get(String columnName)
```


Ottiene i dati memorizzati nella colonna specificata per nome della colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnName | java.lang.String | Il nome della colonna. |

**Returns:**
java.lang.Object -
### getColumns() {#getColumns--}
```
public abstract String[] getColumns()
```


Ottiene il nome delle colonne.

**Returns:**
java.lang.String[]
### getCount() {#getCount--}
```
public abstract int getCount()
```


Ottiene il conteggio dei record. -1 per conteggio dei record sconosciuto.

**Returns:**
int
### next() {#next--}
```
public abstract boolean next()
```


Sposta il cursore di una riga verso il basso dalla sua posizione attuale.

**Returns:**
boolean - se la nuova riga corrente è valida; false se non ci sono più righe
