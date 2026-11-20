---
title: "GridCells"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula una raccolta di oggetti."
type: docs
url: /it/java/com.aspose.gridweb/gridcells/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class GridCells implements Iterable
```

Incapsula una collezione di oggetti [GridCell](../../com.aspose.gridweb/gridcell).
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [cellIndexToName(int row, int column)](#cellIndexToName-int-int-) | Ottiene il nome della cella in base ai suoi indici di riga e colonna. |
| [cellNameToIndex(String cellName, int row, int column)](#cellNameToIndex-java.lang.String-int-int-) | Ottiene gli indici di riga e colonna della cella in base al suo nome |
| [checkCell(int row, int column)](#checkCell-int-int-) | Ottiene l'elemento [GridCell](../../com.aspose.gridweb/gridcell) o null all'indice di riga e colonna della cella specificati. |
| [checkColumn(int col)](#checkColumn-int-) | Ottiene l'elemento [GridColumn](../../com.aspose.gridweb/gridcolumn) o null all'indice di colonna specificato. |
| [checkRow(int i)](#checkRow-int-) | Ottiene l'elemento [GridRow](../../com.aspose.gridweb/gridrow) o null all'indice di riga della cella specificato. |
| [clear()](#clear--) | Cancella tutte le celle nella collezione. |
| [clearContents(GridCellArea range)](#clearContents-com.aspose.gridweb.GridCellArea-) | Cancella il contenuto di un intervallo. |
| [clearContents(int startRow, int startColumn, int endRow, int endColumn)](#clearContents-int-int-int-int-) | Cancella il contenuto di un intervallo. |
| [clearFormats(GridCellArea range)](#clearFormats-com.aspose.gridweb.GridCellArea-) | Cancella la formattazione di un intervallo. |
| [clearFormats(int startRow, int startColumn, int endRow, int endColumn)](#clearFormats-int-int-int-int-) | Cancella la formattazione di un intervallo. |
| [clearRange(GridCellArea range)](#clearRange-com.aspose.gridweb.GridCellArea-) | Cancella il contenuto e la formattazione di un intervallo. |
| [clearRange(int startRow, int startColumn, int endRow, int endColumn)](#clearRange-int-int-int-int-) | Cancella il contenuto e la formattazione di un intervallo. |
| [columnIndexToName(int column)](#columnIndexToName-int-) | Ottiene il nome della colonna in base all'indice della colonna. |
| [columnNameToIndex(String columnName)](#columnNameToIndex-java.lang.String-) | Ottiene l'indice della colonna in base al nome della colonna. |
| [copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex)](#copyColumn-com.aspose.gridweb.GridCells-int-int-) | Copia i dati e la formattazione di un'intera colonna. |
| [copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)](#copyColumns-com.aspose.gridweb.GridCells-int-int-int-) | Copia i dati e la formattazione di un'intera colonna. |
| [copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex)](#copyRow-com.aspose.gridweb.GridCells-int-int-) | Copia i dati e la formattazione di un'intera riga. |
| [copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)](#copyRows-com.aspose.gridweb.GridCells-int-int-int-) | Copia i dati e la formattazione di alcune intere righe. |
| [deleteBlankColumns()](#deleteBlankColumns--) | Elimina tutte le colonne vuote che non contengono alcun dato. |
| [deleteBlankRows()](#deleteBlankRows--) | Elimina tutte le righe vuote che non contengono alcun dato. |
| [deleteColumn(int columnIndex)](#deleteColumn-int-) | Elimina una colonna. |
| [deleteColumn(int columnIndex, boolean updateReference)](#deleteColumn-int-boolean-) | Elimina una colonna. |
| [deleteColumns(int columnIndex, int totalColumns, boolean updateReference)](#deleteColumns-int-int-boolean-) | Elimina diverse colonne. |
| [deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)](#deleteRange-int-int-int-int-int-) | Elimina un intervallo di celle e sposta le celle secondo l'opzione di spostamento. |
| [deleteRow(int rowIndex)](#deleteRow-int-) | Elimina una riga. |
| [deleteRows(int rowIndex, int totalRows)](#deleteRows-int-int-) | Elimina diverse righe. |
| [deleteRows(int rowIndex, int totalRows, boolean updateReference)](#deleteRows-int-int-boolean-) | Elimina più righe nel foglio di lavoro. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportArray-int-int-int-int-) | Esporta i dati nella collezione [GridCells](../../com.aspose.gridweb/gridcells) in un oggetto array bidimensionale. |
| [get(int row, int column)](#get-int-int-) | Ottiene l'elemento [GridCell](../../com.aspose.gridweb/gridcell) all'indice di riga e colonna della cella specificati. |
| [get(String cellName)](#get-java.lang.String-) | Ottiene l'elemento [GridCell](../../com.aspose.gridweb/gridcell) al nome della cella specificato. |
| [getCell(int row, int column)](#getCell-int-int-) | Ottiene l'elemento [GridCell](../../com.aspose.gridweb/gridcell) all'indice di riga e colonna della cella specificati. |
| [getClass()](#getClass--) |  |
| [getColumnWidth(int column)](#getColumnWidth-int-) | Ottiene la larghezza della colonna specificata |
| [getColumnWidthInch(int column)](#getColumnWidthInch-int-) | Ottiene la larghezza della colonna specificata, in unità di pollici. |
| [getColumnWidthPixel(int column)](#getColumnWidthPixel-int-) | Ottiene la larghezza della colonna specificata, in unità di pixel. |
| [getColumns()](#getColumns--) | Ottiene la collezione di oggetti [GridColumn](../../com.aspose.gridweb/gridcolumn) che rappresentano le singole colonne in questo foglio di lavoro. |
| [getCount()](#getCount--) | Ottiene il numero di celle. |
| [getFirstCell()](#getFirstCell--) | Ottiene la prima cella in questo foglio di lavoro. |
| [getLastCell()](#getLastCell--) | Ottiene l'ultima cella in questo foglio di lavoro. |
| [getMaxColumn()](#getMaxColumn--) | Indice massimo di colonna della cella che contiene dati o stile. |
| [getMaxDataColumn()](#getMaxDataColumn--) | Indice massimo della colonna della cella che contiene dati. |
| [getMaxDataRow()](#getMaxDataRow--) | Indice massimo della riga della cella che contiene dati. |
| [getMaxRow()](#getMaxRow--) | Indice massimo della riga della cella che contiene dati o stile. |
| [getMergedCells()](#getMergedCells--) | Ottiene la raccolta delle celle unite. |
| [getMinColumn()](#getMinColumn--) | Indice minimo di colonna di quelle celle che sono state istanziate nella raccolta (non include la colonna in cui lo stile è definito per l'intera colonna ma non è stata istanziata alcuna cella). |
| [getMinDataColumn()](#getMinDataColumn--) | Indice minimo di colonna della cella che contiene dati. |
| [getMinDataRow()](#getMinDataRow--) | Indice minimo di riga della cella che contiene dati. |
| [getMinRow()](#getMinRow--) | Indice minimo di riga della cella che contiene dati o stile. |
| [getRow(int i)](#getRow-int-) | Ottiene l'elemento [GridRow](../../com.aspose.gridweb/gridrow) all'indice di riga della cella specificato. |
| [getRowEnumerator()](#getRowEnumerator--) | Restituisce l'enumeratore delle righe |
| [getRowHeight(int row)](#getRowHeight-int-) | Ottiene l'altezza di una riga specificata. |
| [getRowHeightInch(int row)](#getRowHeightInch-int-) | Ottiene l'altezza di una riga specificata in unità di pollici. |
| [getRowHeightPixel(int row)](#getRowHeightPixel-int-) | Ottiene l'altezza di una riga specificata in unità di pixel. |
| [getRowOutlineLevel(int rowIndex)](#getRowOutlineLevel-int-) | Ottiene il livello di contorno della riga. |
| [getRows()](#getRows--) | Ottiene la collezione di oggetti [GridRow](../../com.aspose.gridweb/gridrow) che rappresentano le singole righe in questo foglio di lavoro. |
| [getStandardHeight()](#getStandardHeight--) | Ottiene l'altezza predefinita della riga in questo foglio di lavoro, in unità di punti. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Ottiene l'altezza predefinita della riga in questo foglio di lavoro, in unità di pixel. |
| [getStandardWidth()](#getStandardWidth--) | Ottiene la larghezza predefinita della colonna nel foglio di lavoro, in unità di caratteri. |
| [getStandardWidthInch()](#getStandardWidthInch--) | Ottiene la larghezza predefinita delle colonne nel foglio di lavoro, in unità di pollici. |
| [getStandardWidthPixels()](#getStandardWidthPixels--) | Ottiene la larghezza predefinita delle colonne nel foglio di lavoro, in unità di pixel. |
| [getViewColumnWidthPixel(int column)](#getViewColumnWidthPixel-int-) | Ottieni la larghezza in diversi tipi di visualizzazione. |
| [groupColumns(int firstIndex, int lastIndex)](#groupColumns-int-int-) | Raggruppa le colonne. |
| [groupColumns(int firstIndex, int lastIndex, boolean isHidden)](#groupColumns-int-int-boolean-) | Raggruppa le colonne. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Raggruppa le righe. |
| [hashCode()](#hashCode--) |  |
| [hideColumn(int column)](#hideColumn-int-) | Nasconde una colonna. |
| [hideRow(int row)](#hideRow-int-) | Nasconde una riga. |
| [insertColumn(int columnIndex)](#insertColumn-int-) | Inserisce una nuova colonna nel foglio di lavoro. |
| [insertColumn(int columnIndex, boolean updateReference)](#insertColumn-int-boolean-) | Inserisce una nuova colonna nel foglio di lavoro. |
| [insertColumns(int columnIndex, int totalColumns)](#insertColumns-int-int-) | Inserisce alcune colonne nel foglio di lavoro. |
| [insertColumns(int columnIndex, int totalColumns, boolean updateReference)](#insertColumns-int-int-boolean-) | Inserisce alcune colonne nel foglio di lavoro. |
| [insertRange(GridCellArea area, int shiftType)](#insertRange-com.aspose.gridweb.GridCellArea-int-) | Inserisce un intervallo di celle e sposta le celle in base all'opzione di spostamento. |
| [insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference)](#insertRange-com.aspose.gridweb.GridCellArea-int-int-boolean-) | Inserisce un intervallo di celle e sposta le celle in base all'opzione di spostamento. |
| [insertRow(int rowIndex)](#insertRow-int-) | Inserisce una nuova riga nel foglio di lavoro. |
| [insertRows(int rowIndex, int totalRows)](#insertRows-int-int-) | Inserisce più righe nel foglio di lavoro. |
| [insertRows(int rowIndex, int totalRows, boolean updateReference)](#insertRows-int-int-boolean-) | Inserisce più righe nel foglio di lavoro. |
| [isBlankColumn(int columnIndex)](#isBlankColumn-int-) | Verifica se la colonna specificata è vuota (non contiene alcun dato). |
| [isColumnHidden(int columnIndex)](#isColumnHidden-int-) | Verifica se una colonna all'indice specificato è nascosta. |
| [isRowHidden(int rowIndex)](#isRowHidden-int-) | Verifica se una riga all'indice specificato è nascosta. |
| [iterator()](#iterator--) | Restituisce l'enumeratore delle righe |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#merge-int-int-int-int-) | Unisce un intervallo specificato di celle in una singola cella. |
| [moveRange(GridCellArea sourceArea, int destRow, int destColumn)](#moveRange-com.aspose.gridweb.GridCellArea-int-int-) | Sposta l'intervallo. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)](#removeDuplicates-int-int-int-int-) | Rimuove i valori duplicati nell'intervallo. |
| [removeFormulas()](#removeFormulas--) | Rimuove tutte le formule e le sostituisce con il valore della formula. |
| [setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle)](#setBorders-int-int-int-int-int-com.aspose.gridweb.WebBorderStyle-) | Imposta i bordi per un intervallo di celle. |
| [setColumnWidth(int column, double width)](#setColumnWidth-int-double-) | Imposta la larghezza della colonna specificata. |
| [setColumnWidthInch(int column, double inches)](#setColumnWidthInch-int-double-) | Imposta la larghezza della colonna in unità di pollici. |
| [setColumnWidthPixel(int column, int pixel)](#setColumnWidthPixel-int-int-) | Imposta la larghezza della colonna in unità di pixel. |
| [setRowHeight(int row, double height)](#setRowHeight-int-double-) | Imposta l'altezza della riga specificata. |
| [setRowHeightInch(int row, double inches)](#setRowHeightInch-int-double-) | Imposta l'altezza della riga in unità di pollici. |
| [setRowHeightPixel(int row, int pixels)](#setRowHeightPixel-int-int-) | Imposta l'altezza della riga in unità di pixel. |
| [setRowOutlineLevel(int rowIndex, int outlineLevel)](#setRowOutlineLevel-int-int-) | Imposta il livello di contorno della riga. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di punti. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di pixel. |
| [setStandardWidth(double value)](#setStandardWidth-double-) | Imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di caratteri. |
| [setStandardWidthInch(double value)](#setStandardWidthInch-double-) | Imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di pollici. |
| [setStandardWidthPixels(int value)](#setStandardWidthPixels-int-) | Imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di pixel. |
| [setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style)](#setStyle-int-int-int-int-com.aspose.gridweb.GridTableItemStyle-) | Imposta lo stile a un intervallo di celle specificato. |
| [setStyle(String cellRange, GridTableItemStyle style)](#setStyle-java.lang.String-com.aspose.gridweb.GridTableItemStyle-) | Imposta lo stile a un intervallo di celle specificato. |
| [sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright)](#sort-int-int-int-int-int-boolean-boolean-boolean-) | Ordina i dati in ordine ascendente/descendente dall'alto verso il basso in un intervallo di un foglio di lavoro per indice di colonna specificato. |
| [sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive)](#sort-int-int-int-int-int---int---int-boolean-) | Ordina i dati in ordine ascendente/descendente dall'alto verso il basso in un intervallo di un foglio di lavoro per indice di colonna specificato. |
| [toString()](#toString--) |  |
| [unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#unMerge-int-int-int-int-) | Separa un intervallo specificato di celle unite. |
| [ungroupColumns(int firstIndex, int lastIndex)](#ungroupColumns-int-int-) | Separa le colonne. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Separa le righe. |
| [unhideColumn(int column, double width)](#unhideColumn-int-double-) | Rivela una colonna |
| [unhideRow(int row)](#unhideRow-int-) | Rivela una riga. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### cellIndexToName(int row, int column) {#cellIndexToName-int-int-}
```
public static String cellIndexToName(int row, int column)
```


Ottiene il nome della cella in base ai suoi indici di riga e colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |
| colonna | int | Indice di colonna. |

**Returns:**
java.lang.String - Nome della cella.
### cellNameToIndex(String cellName, int row, int column) {#cellNameToIndex-java.lang.String-int-int-}
```
public static void cellNameToIndex(String cellName, int row, int column)
```


Ottiene gli indici di riga e colonna della cella in base al suo nome

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | java.lang.String | Nome della cella. |
| riga | int | Indice della riga di output |
| colonna | int | Indice della colonna di output |

### checkCell(int row, int column) {#checkCell-int-int-}
```
public GridCell checkCell(int row, int column)
```


Ottiene l'elemento [GridCell](../../com.aspose.gridweb/gridcell) o null all'indice di riga e colonna della cella specificati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice della riga |
| colonna | int | Indice della colonna |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - Return GridCell object if a GridCell object exists. Return null if the GridCell does not exist.
### checkColumn(int col) {#checkColumn-int-}
```
public GridColumn checkColumn(int col)
```


Ottiene l'elemento [GridColumn](../../com.aspose.gridweb/gridcolumn) o null all'indice di colonna specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| col | int | L'indice della colonna. |

**Returns:**
[GridColumn](../../com.aspose.gridweb/gridcolumn) - The Column object.
### checkRow(int i) {#checkRow-int-}
```
public GridRow checkRow(int i)
```


Ottiene l'elemento [GridRow](../../com.aspose.gridweb/gridrow) o null all'indice di riga della cella specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| i | int | Indice della riga |

**Returns:**
[GridRow](../../com.aspose.gridweb/gridrow) - Returns [GridRow](../../com.aspose.gridweb/gridrow) object If the row object does exist, otherwise returns null.
### clear() {#clear--}
```
public void clear()
```


Cancella tutte le celle nella collezione.

### clearContents(GridCellArea range) {#clearContents-com.aspose.gridweb.GridCellArea-}
```
public void clearContents(GridCellArea range)
```


Cancella il contenuto di un intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Intervallo da cancellare. |

### clearContents(int startRow, int startColumn, int endRow, int endColumn) {#clearContents-int-int-int-int-}
```
public void clearContents(int startRow, int startColumn, int endRow, int endColumn)
```


Cancella il contenuto di un intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Indice della riga di inizio. |
| startColumn | int | Indice della colonna di inizio. |
| endRow | int | Indice della riga finale. |
| endColumn | int | Indice della colonna finale. |

### clearFormats(GridCellArea range) {#clearFormats-com.aspose.gridweb.GridCellArea-}
```
public void clearFormats(GridCellArea range)
```


Cancella la formattazione di un intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Intervallo da cancellare. |

### clearFormats(int startRow, int startColumn, int endRow, int endColumn) {#clearFormats-int-int-int-int-}
```
public void clearFormats(int startRow, int startColumn, int endRow, int endColumn)
```


Cancella la formattazione di un intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Indice della riga di inizio. |
| startColumn | int | Indice della colonna di inizio. |
| endRow | int | Indice della riga finale. |
| endColumn | int | Indice della colonna finale. |

### clearRange(GridCellArea range) {#clearRange-com.aspose.gridweb.GridCellArea-}
```
public void clearRange(GridCellArea range)
```


Cancella il contenuto e la formattazione di un intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Intervallo da cancellare. |

### clearRange(int startRow, int startColumn, int endRow, int endColumn) {#clearRange-int-int-int-int-}
```
public void clearRange(int startRow, int startColumn, int endRow, int endColumn)
```


Cancella il contenuto e la formattazione di un intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Indice della riga di inizio. |
| startColumn | int | Indice della colonna di inizio. |
| endRow | int | Indice della riga finale. |
| endColumn | int | Indice della colonna finale. |

### columnIndexToName(int column) {#columnIndexToName-int-}
```
public static String columnIndexToName(int column)
```


Ottiene il nome della colonna in base all'indice della colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice di colonna. |

**Returns:**
java.lang.String - Nome della colonna.
### columnNameToIndex(String columnName) {#columnNameToIndex-java.lang.String-}
```
public static int columnNameToIndex(String columnName)
```


Ottiene l'indice della colonna in base al nome della colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnName | java.lang.String | Nome della colonna. |

**Returns:**
int - Indice di colonna.
### copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex) {#copyColumn-com.aspose.gridweb.GridCells-int-int-}
```
public void copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```


Copia i dati e la formattazione di un'intera colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | L'oggetto Source Cells contiene dati e formattazioni da copiare. |
| sourceColumnIndex | int | Indice della colonna di origine. |
| destinationColumnIndex | int | Indice della colonna di destinazione. |

### copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber) {#copyColumns-com.aspose.gridweb.GridCells-int-int-int-}
```
public void copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)
```


Copia i dati e la formattazione di un'intera colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | L'oggetto Source Cells contiene dati e formattazioni da copiare. |
| sourceColumnIndex | int | Indice della colonna di origine. |
| destinationColumnIndex | int | Indice della colonna di destinazione. |
| columnNumber | int | Il numero della colonna copiata. |

### copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex) {#copyRow-com.aspose.gridweb.GridCells-int-int-}
```
public void copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex)
```


Copia i dati e la formattazione di un'intera riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | L'oggetto Source Cells contiene dati e formattazioni da copiare. |
| sourceRowIndex | int | Indice della riga di origine. |
| destinationRowIndex | int | Indice della riga di destinazione. |

### copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber) {#copyRows-com.aspose.gridweb.GridCells-int-int-int-}
```
public void copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```


Copia i dati e la formattazione di alcune intere righe.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | L'oggetto Source Cells contiene dati e formattazioni da copiare. |
| sourceRowIndex | int | Indice della riga di origine. |
| destinationRowIndex | int | Indice della riga di destinazione. |
| rowNumber | int | Il numero della riga copiata. |

### deleteBlankColumns() {#deleteBlankColumns--}
```
public void deleteBlankColumns()
```


Elimina tutte le colonne vuote che non contengono alcun dato.

### deleteBlankRows() {#deleteBlankRows--}
```
public void deleteBlankRows()
```


Elimina tutte le righe vuote che non contengono alcun dato.

### deleteColumn(int columnIndex) {#deleteColumn-int-}
```
public void deleteColumn(int columnIndex)
```


Elimina una colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice di colonna. |

### deleteColumn(int columnIndex, boolean updateReference) {#deleteColumn-int-boolean-}
```
public void deleteColumn(int columnIndex, boolean updateReference)
```


Elimina una colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice di colonna. |
| updateReference | boolean | Indica se aggiornare i riferimenti in altri fogli di lavoro. |

### deleteColumns(int columnIndex, int totalColumns, boolean updateReference) {#deleteColumns-int-int-boolean-}
```
public void deleteColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Elimina diverse colonne.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice di colonna. |
| totalColumns | int | Numero di colonne da eliminare. |
| updateReference | boolean | Indica se aggiornare i riferimenti in altri fogli di lavoro. |

### deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType) {#deleteRange-int-int-int-int-int-}
```
public void deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)
```


Elimina un intervallo di celle e sposta le celle secondo l'opzione di spostamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Indice della riga di inizio. |
| startColumn | int | Indice della colonna di inizio. |
| endRow | int | Indice della riga finale. |
| endColumn | int | Indice della colonna finale. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Opzione di spostamento delle celle. |

### deleteRow(int rowIndex) {#deleteRow-int-}
```
public void deleteRow(int rowIndex)
```


Elimina una riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | Indice di riga. |

### deleteRows(int rowIndex, int totalRows) {#deleteRows-int-int-}
```
public boolean deleteRows(int rowIndex, int totalRows)
```


Elimina diverse righe.

**Remarks**

Se l'intervallo eliminato contiene la parte superiore (non l'intero) della tabella (ListObject), l'intervallo non può essere eliminato e non verrà eseguita alcuna operazione. Funziona come MS Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | L'indice della prima riga da eliminare. |
| totalRows | int | Numero di righe da eliminare. |

**Returns:**
boolean
### deleteRows(int rowIndex, int totalRows, boolean updateReference) {#deleteRows-int-int-boolean-}
```
public boolean deleteRows(int rowIndex, int totalRows, boolean updateReference)
```


Elimina più righe nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | Indice di riga. |
| totalRows | int | Numero di righe da eliminare. |
| updateReference | boolean | Indica se aggiornare i riferimenti in altri fogli di lavoro. |

**Returns:**
boolean -
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportArray-int-int-int-int-}
```
public Object[][] exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Esporta i dati nella collezione [GridCells](../../com.aspose.gridweb/gridcells) in un oggetto array bidimensionale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | int | Il numero di riga della prima cella da esportare. |
| firstColumn | int | Il numero di colonna della prima cella da esportare. |
| totalRows | int | Numero di righe da esportare |
| totalColumns | int | Numero di colonne da esportare |

**Returns:**
java.lang.Object[][] - Oggetto array dei valori delle celle esportate.
### get(int row, int column) {#get-int-int-}
```
public GridCell get(int row, int column)
```


Ottiene l'elemento [GridCell](../../com.aspose.gridweb/gridcell) all'indice di riga e colonna della cella specificati.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridCells cells = GridWeb1.getWorkSheets().get(0).getCells();
         //Gets the cell at "A1"
         GridCell cell = cells.get(0, 0);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |
| colonna | int | Indice di colonna. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - The [GridCell](../../com.aspose.gridweb/gridcell) object.
### get(String cellName) {#get-java.lang.String-}
```
public GridCell get(String cellName)
```


Ottiene l'elemento [GridCell](../../com.aspose.gridweb/gridcell) al nome della cella specificato.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
          GridCells cells = GridWeb1.getWorkSheets().get(0).getCells();
          GridCell cell = cells.get("A1");	//Gets the cell at "A1"
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | java.lang.String | Nome della cella, includendo la lettera della colonna e il numero della riga, ad esempio A5. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - A [GridCell](../../com.aspose.gridweb/gridcell) object
### getCell(int row, int column) {#getCell-int-int-}
```
public GridCell getCell(int row, int column)
```


Ottiene l'elemento [GridCell](../../com.aspose.gridweb/gridcell) all'indice di riga e colonna della cella specificati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice della riga |
| colonna | int | Indice della colonna |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - Return Cell object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnWidth(int column) {#getColumnWidth-int-}
```
public double getColumnWidth(int column)
```


Ottiene la larghezza della colonna specificata

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice della colonna |

**Returns:**
double - Larghezza della colonna
### getColumnWidthInch(int column) {#getColumnWidthInch-int-}
```
public double getColumnWidthInch(int column)
```


Ottiene la larghezza della colonna specificata, in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice della colonna |

**Returns:**
double - Larghezza della colonna
### getColumnWidthPixel(int column) {#getColumnWidthPixel-int-}
```
public int getColumnWidthPixel(int column)
```


Ottiene la larghezza della colonna specificata, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice della colonna |

**Returns:**
int - Larghezza della colonna nella visualizzazione normale.
### getColumns() {#getColumns--}
```
public GridColumnCollection getColumns()
```


Ottiene la collezione di oggetti [GridColumn](../../com.aspose.gridweb/gridcolumn) che rappresentano le singole colonne in questo foglio di lavoro.

**Returns:**
[GridColumnCollection](../../com.aspose.gridweb/gridcolumncollection)
### getCount() {#getCount--}
```
public int getCount()
```


Ottiene il numero di celle.

**Returns:**
int
### getFirstCell() {#getFirstCell--}
```
public GridCell getFirstCell()
```


Ottiene la prima cella in questo foglio di lavoro.

**Remarks**

Restituisce null se non ci sono dati nel foglio di lavoro.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getLastCell() {#getLastCell--}
```
public GridCell getLastCell()
```


Ottiene l'ultima cella in questo foglio di lavoro.

**Remarks**

Restituisce null se non ci sono dati nel foglio di lavoro.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Indice massimo di colonna della cella che contiene dati o stile.

**Remarks**

Restituisce -1 se non c'è alcuna cella.

**Returns:**
int
### getMaxDataColumn() {#getMaxDataColumn--}
```
public int getMaxDataColumn()
```


Indice massimo della colonna della cella che contiene dati.

**Remarks**

-1 verrà restituito se non esiste alcuna cella che contiene dati. Questa proprietà deve iterare e controllare tutte le celle in un foglio di lavoro, quindi è un processo che richiede tempo e non dovrebbe essere invocata ripetutamente.

**Returns:**
int
### getMaxDataRow() {#getMaxDataRow--}
```
public int getMaxDataRow()
```


Indice massimo della riga della cella che contiene dati.

**Remarks**

Restituisce -1 se non esiste alcuna cella che contiene dati.

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Indice massimo della riga della cella che contiene dati o stile.

**Remarks**

Restituisce -1 se non esiste alcuna cella che contiene dati o stile nel foglio di lavoro.

**Returns:**
int
### getMergedCells() {#getMergedCells--}
```
public ArrayList getMergedCells()
```


Ottiene la raccolta delle celle unite.

**Remarks**

In questa collezione, ogni elemento è una struttura [GridCellArea](../../com.aspose.gridweb/gridcellarea) che rappresenta un'area di celle unite.

**Returns:**
java.util.ArrayList
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Indice minimo di colonna di quelle celle che sono state istanziate nella raccolta (non include la colonna in cui lo stile è definito per l'intera colonna ma non è stata istanziata alcuna cella).

**Returns:**
int
### getMinDataColumn() {#getMinDataColumn--}
```
public int getMinDataColumn()
```


Indice minimo di colonna della cella che contiene dati.

**Remarks**

-1 verrà restituito se non esiste alcuna cella che contiene dati. Questa proprietà deve iterare e controllare tutte le celle in un foglio di lavoro, quindi è un processo che richiede tempo e non dovrebbe essere invocata ripetutamente.

**Returns:**
int
### getMinDataRow() {#getMinDataRow--}
```
public int getMinDataRow()
```


Indice minimo di riga della cella che contiene dati.

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


Indice minimo di riga della cella che contiene dati o stile.

**Returns:**
int
### getRow(int i) {#getRow-int-}
```
public GridRow getRow(int i)
```


Ottiene l'elemento [GridRow](../../com.aspose.gridweb/gridrow) all'indice di riga della cella specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| i | int | Indice della riga |

**Returns:**
[GridRow](../../com.aspose.gridweb/gridrow) - the row object
### getRowEnumerator() {#getRowEnumerator--}
```
public Iterator getRowEnumerator()
```


Restituisce l'enumeratore delle righe

**Returns:**
java.util.Iterator - L'enumeratore delle righe.
### getRowHeight(int row) {#getRowHeight-int-}
```
public double getRowHeight(int row)
```


Ottiene l'altezza di una riga specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice della riga |

**Returns:**
double - Altezza della riga
### getRowHeightInch(int row) {#getRowHeightInch-int-}
```
public double getRowHeightInch(int row)
```


Ottiene l'altezza di una riga specificata in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice della riga |

**Returns:**
double - Altezza della riga
### getRowHeightPixel(int row) {#getRowHeightPixel-int-}
```
public int getRowHeightPixel(int row)
```


Ottiene l'altezza di una riga specificata in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice della riga |

**Returns:**
int - Altezza della riga
### getRowOutlineLevel(int rowIndex) {#getRowOutlineLevel-int-}
```
public int getRowOutlineLevel(int rowIndex)
```


Ottiene il livello di contorno della riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | indice di riga. |

**Returns:**
int - il livello di contorno.
### getRows() {#getRows--}
```
public GridRowCollection getRows()
```


Ottiene la collezione di oggetti [GridRow](../../com.aspose.gridweb/gridrow) che rappresentano le singole righe in questo foglio di lavoro.

**Returns:**
[GridRowCollection](../../com.aspose.gridweb/gridrowcollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


Ottiene l'altezza predefinita della riga in questo foglio di lavoro, in unità di punti.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


Ottiene l'altezza predefinita della riga in questo foglio di lavoro, in unità di pixel.

**Returns:**
int
### getStandardWidth() {#getStandardWidth--}
```
public double getStandardWidth()
```


Ottiene la larghezza predefinita della colonna nel foglio di lavoro, in unità di caratteri.

**Returns:**
double
### getStandardWidthInch() {#getStandardWidthInch--}
```
public double getStandardWidthInch()
```


Ottiene la larghezza predefinita delle colonne nel foglio di lavoro, in unità di pollici.

**Returns:**
double
### getStandardWidthPixels() {#getStandardWidthPixels--}
```
public int getStandardWidthPixels()
```


Ottiene la larghezza predefinita delle colonne nel foglio di lavoro, in unità di pixel.

**Returns:**
int
### getViewColumnWidthPixel(int column) {#getViewColumnWidthPixel-int-}
```
public int getViewColumnWidthPixel(int column)
```


Ottieni la larghezza in diversi tipi di visualizzazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | L'indice della colonna. |

**Returns:**
int - la larghezza della colonna in unità di pixel
### groupColumns(int firstIndex, int lastIndex) {#groupColumns-int-int-}
```
public void groupColumns(int firstIndex, int lastIndex)
```


Raggruppa le colonne.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | int | Il primo indice di colonna da raggruppare. |
| lastIndex | int | L'ultimo indice di colonna da raggruppare. |

### groupColumns(int firstIndex, int lastIndex, boolean isHidden) {#groupColumns-int-int-boolean-}
```
public void groupColumns(int firstIndex, int lastIndex, boolean isHidden)
```


Raggruppa le colonne.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | int | Il primo indice di colonna da raggruppare. |
| lastIndex | int | L'ultimo indice di colonna da raggruppare. |
| isHidden | boolean | Specifica se le colonne raggruppate sono nascoste. |

### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


Raggruppa le righe.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | int | Il primo indice di riga da raggruppare. |
| lastIndex | int | L'ultimo indice di riga da raggruppare. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideColumn(int column) {#hideColumn-int-}
```
public void hideColumn(int column)
```


Nasconde una colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice di colonna. |

### hideRow(int row) {#hideRow-int-}
```
public void hideRow(int row)
```


Nasconde una riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |

### insertColumn(int columnIndex) {#insertColumn-int-}
```
public void insertColumn(int columnIndex)
```


Inserisce una nuova colonna nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice di colonna. |

### insertColumn(int columnIndex, boolean updateReference) {#insertColumn-int-boolean-}
```
public void insertColumn(int columnIndex, boolean updateReference)
```


Inserisce una nuova colonna nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice di colonna. |
| updateReference | boolean | Indica se i riferimenti in altri fogli di lavoro saranno aggiornati. |

### insertColumns(int columnIndex, int totalColumns) {#insertColumns-int-int-}
```
public void insertColumns(int columnIndex, int totalColumns)
```


Inserisce alcune colonne nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice di colonna. |
| totalColumns | int | Il numero di colonne. |

### insertColumns(int columnIndex, int totalColumns, boolean updateReference) {#insertColumns-int-int-boolean-}
```
public void insertColumns(int columnIndex, int totalColumns, boolean updateReference)
```


Inserisce alcune colonne nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice di colonna. |
| totalColumns | int | Il numero di colonne. |
| updateReference | boolean | Indica se i riferimenti in altri fogli di lavoro saranno aggiornati. |

### insertRange(GridCellArea area, int shiftType) {#insertRange-com.aspose.gridweb.GridCellArea-int-}
```
public void insertRange(GridCellArea area, int shiftType)
```


Inserisce un intervallo di celle e sposta le celle in base all'opzione di spostamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Sposta area. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Opzione di spostamento delle celle. |

### insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference) {#insertRange-com.aspose.gridweb.GridCellArea-int-int-boolean-}
```
public void insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference)
```


Inserisce un intervallo di celle e sposta le celle in base all'opzione di spostamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Sposta area. |
| shiftNumber | int | Numero di righe o colonne da inserire. |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype). Opzione di spostamento delle celle. |
| updateReference | boolean | Indica se aggiornare i riferimenti in altri fogli di lavoro. |

### insertRow(int rowIndex) {#insertRow-int-}
```
public void insertRow(int rowIndex)
```


Inserisce una nuova riga nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | Indice di riga. |

### insertRows(int rowIndex, int totalRows) {#insertRows-int-int-}
```
public void insertRows(int rowIndex, int totalRows)
```


Inserisce più righe nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | Indice di riga. |
| totalRows | int | Numero di righe da inserire. |

### insertRows(int rowIndex, int totalRows, boolean updateReference) {#insertRows-int-int-boolean-}
```
public void insertRows(int rowIndex, int totalRows, boolean updateReference)
```


Inserisce più righe nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | Indice di riga. |
| totalRows | int | Numero di righe da inserire. |
| updateReference | boolean | Indica se i riferimenti in altri fogli di lavoro saranno aggiornati. |

### isBlankColumn(int columnIndex) {#isBlankColumn-int-}
```
public boolean isBlankColumn(int columnIndex)
```


Verifica se la colonna specificata è vuota (non contiene alcun dato).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | l'indice della colonna |

**Returns:**
boolean - true se la colonna specificata non contiene alcun dato
### isColumnHidden(int columnIndex) {#isColumnHidden-int-}
```
public boolean isColumnHidden(int columnIndex)
```


Verifica se una colonna all'indice specificato è nascosta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | indice della colonna |

**Returns:**
boolean - true se la colonna è nascosta.
### isRowHidden(int rowIndex) {#isRowHidden-int-}
```
public boolean isRowHidden(int rowIndex)
```


Verifica se una riga all'indice specificato è nascosta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | indice di riga |

**Returns:**
boolean - true se la riga è nascosta
### iterator() {#iterator--}
```
public Iterator iterator()
```


Restituisce l'enumeratore delle righe

**Returns:**
java.util.Iterator - L'enumeratore delle righe
### merge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#merge-int-int-int-int-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Unisce un intervallo specificato di celle in una singola cella.

**Remarks**

Fai riferimento alla cella unita tramite l'indirizzo della cella in alto a sinistra nell'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | int | Prima riga di questo intervallo(basato su zero) |
| firstColumn | int | Prima colonna di questo intervallo(basato su zero) |
| totalRows | int | Numero di righe(basato su uno) |
| totalColumns | int | Numero di colonne (basato su 1) |

### moveRange(GridCellArea sourceArea, int destRow, int destColumn) {#moveRange-com.aspose.gridweb.GridCellArea-int-int-}
```
public void moveRange(GridCellArea sourceArea, int destRow, int destColumn)
```


Sposta l'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | L'intervallo che dovrebbe essere spostato. |
| destRow | int | La riga di destinazione. |
| destColumn | int | La colonna di destinazione. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn) {#removeDuplicates-int-int-int-int-}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```


Rimuove i valori duplicati nell'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Riga di inizio. |
| startColumn | int | Colonna di inizio |
| endRow | int | L'indice della riga finale. |
| endColumn | int | L'indice della colonna finale. |

### removeFormulas() {#removeFormulas--}
```
public void removeFormulas()
```


Rimuove tutte le formule e le sostituisce con il valore della formula.

### setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle) {#setBorders-int-int-int-int-int-com.aspose.gridweb.WebBorderStyle-}
```
public void setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle)
```


Imposta i bordi per un intervallo di celle.

**Example**

```
           GridWeb GridWeb1 = new GridWeb();
           WebBorderStyle borderStyle1 = new WebBorderStyle();
         	 GridWeb1.getWorkSheets().get(0).getCells().setBorders(0, 0, 5, 8, SetBorderPosition.OUTLINE, borderStyle1);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | int | Il numero della prima riga dell'intervallo (basato su zero). |
| firstColumn | int | Il numero della prima colonna dell'intervallo (basato su zero). |
| rowNumber | int | Il numero di righe. |
| columnNumber | int | Il numero di colonne. |
| position | int | [SetBorderPosition](../../com.aspose.gridweb/setborderposition). La posizione del bordo. |
| borderStyle | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) | Lo stile del bordo. |

### setColumnWidth(int column, double width) {#setColumnWidth-int-double-}
```
public void setColumnWidth(int column, double width)
```


Imposta la larghezza della colonna specificata.

**Remarks**

Per nascondere una colonna, imposta la larghezza della colonna a zero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice di colonna. |
| larghezza | double | Larghezza della colonna. La larghezza della colonna deve essere compresa tra 0 e 255. |

### setColumnWidthInch(int column, double inches) {#setColumnWidthInch-int-double-}
```
public void setColumnWidthInch(int column, double inches)
```


Imposta la larghezza della colonna in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice di colonna. |
| pollici | double | Numero di pollici. |

### setColumnWidthPixel(int column, int pixel) {#setColumnWidthPixel-int-int-}
```
public void setColumnWidthPixel(int column, int pixel)
```


Imposta la larghezza della colonna in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice di colonna. |
| pixel | int | Numero di pixel. |

### setRowHeight(int row, double height) {#setRowHeight-int-double-}
```
public void setRowHeight(int row, double height)
```


Imposta l'altezza della riga specificata.

**Remarks**

Per nascondere una riga, imposta l'altezza della riga a zero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |
| altezza | double | Altezza della riga. In unità di punto deve essere compresa tra 0 e 409,5. |

### setRowHeightInch(int row, double inches) {#setRowHeightInch-int-double-}
```
public void setRowHeightInch(int row, double inches)
```


Imposta l'altezza della riga in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |
| pollici | double | Numero di pollici. Deve essere compreso tra 0 e 409.5/72. |

### setRowHeightPixel(int row, int pixels) {#setRowHeightPixel-int-int-}
```
public void setRowHeightPixel(int row, int pixels)
```


Imposta l'altezza della riga in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |
| pixel | int | Numero di pixel. |

### setRowOutlineLevel(int rowIndex, int outlineLevel) {#setRowOutlineLevel-int-int-}
```
public void setRowOutlineLevel(int rowIndex, int outlineLevel)
```


Imposta il livello di contorno della riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | indice di riga. |
| outlineLevel | int | livello di contorno. |

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


Imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


Imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setStandardWidth(double value) {#setStandardWidth-double-}
```
public void setStandardWidth(double value)
```


Imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di caratteri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setStandardWidthInch(double value) {#setStandardWidthInch-double-}
```
public void setStandardWidthInch(double value)
```


Imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setStandardWidthPixels(int value) {#setStandardWidthPixels-int-}
```
public void setStandardWidthPixels(int value)
```


Imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style) {#setStyle-int-int-int-int-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style)
```


Imposta lo stile a un intervallo di celle specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | int | Prima riga di questo intervallo(basato su zero) |
| firstColumn | int | Prima colonna di questo intervallo(basato su zero) |
| rowNumber | int | Numero di righe(basato su uno) |
| columnNumber | int | Numero di colonne (basato su 1) |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | L'oggetto stile da impostare |

### setStyle(String cellRange, GridTableItemStyle style) {#setStyle-java.lang.String-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(String cellRange, GridTableItemStyle style)
```


Imposta lo stile a un intervallo di celle specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellRange | java.lang.String | L'intervallo dei nomi delle celle, ad esempio "A1:D6" |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | L'oggetto stile da impostare |

### sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright) {#sort-int-int-int-int-int-boolean-boolean-boolean-}
```
public void sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright)
```


Ordina i dati in modo ascendente/decrescente dall'alto verso il basso in un intervallo di un foglio di lavoro secondo l'indice di colonna specificato. Ordina i dati in modo ascendente/decrescente da sinistra a destra in un intervallo di un foglio di lavoro secondo l'indice di riga specificato.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWeb1.getWorkSheets().get(0).getCells().sort(1,0,25,6,3,true,true,false);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Il numero di riga della prima cella da ordinare. |
| startColumn | int | Il numero di colonna della prima cella da ordinare. |
| righe | int | Numero di righe da importare. |
| colonne | int | Numero di colonne da importare. |
| indice | int | L'indice di colonna che specifica la colonna di ordinamento. Se l'orientamento è dall'alto verso il basso, rappresenta l'indice di colonna che specifica la colonna di ordinamento. Se l'orientamento è da sinistra a destra, rappresenta l'indice di riga che specifica la riga di ordinamento. |
| isAsending | boolean | se l'ordine di ordinamento è ascendente . |
| isCaseSensitive | boolean | se l'ordinamento è sensibile al maiuscolo/minuscolo . |
| islefttoright | boolean | se l'orientamento dell'ordinamento è da sinistra a destra |

### sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive) {#sort-int-int-int-int-int---int---int-boolean-}
```
public void sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive)
```


Ordina i dati in modo ascendente/decrescente dall'alto verso il basso in un intervallo di un foglio di lavoro secondo l'indice di colonna specificato. Ordina i dati in modo ascendente/decrescente da sinistra a destra in un intervallo di un foglio di lavoro secondo l'indice di riga specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Il numero di riga della prima cella da ordinare. |
| startColumn | int | Il numero di colonna della prima cella da ordinare. |
| righe | int | Numero di righe da importare. |
| colonne | int | Numero di colonne da importare. |
| indici | int[] | L'array di indici di colonna che specifica la colonna di ordinamento. se l'Orientation è dall'alto verso il basso, rappresenta l'indice di colonna che specifica la colonna di ordinamento. se l'Orientation è da sinistra a destra, rappresenta l'indice di riga che specifica la riga di ordinamento. |
| orders | int[] | [SortByOrder](../../com.aspose.gridweb/sortbyorder). l'array dell'ordine di ordinamento . |
| orientation | int | [SortOrientation](../../com.aspose.gridweb/sortorientation). orientamento di ordinamento |
| isCaseSensitive | boolean | se l'ordinamento è sensibile al maiuscolo/minuscolo . |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#unMerge-int-int-int-int-}
```
public void unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


Separa un intervallo specificato di celle unite.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | int | Prima riga di questo intervallo(basato su zero) |
| firstColumn | int | Prima colonna di questo intervallo(basato su zero) |
| totalRows | int | Numero di righe(basato su uno) |
| totalColumns | int | Numero di colonne (basato su 1) |

### ungroupColumns(int firstIndex, int lastIndex) {#ungroupColumns-int-int-}
```
public void ungroupColumns(int firstIndex, int lastIndex)
```


Separa le colonne.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | int | Il primo indice di colonna da separare. |
| lastIndex | int | L'ultimo indice di colonna da separare. |

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


Separa le righe.

**Remarks**

Rimuove solo le informazioni del gruppo esterno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | int | Il primo indice di riga da separare. |
| lastIndex | int | L'ultimo indice di riga da separare. |

### unhideColumn(int column, double width) {#unhideColumn-int-double-}
```
public void unhideColumn(int column, double width)
```


Rivela una colonna

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice di colonna. |
| larghezza | double | Larghezza colonna..La larghezza della colonna deve essere compresa tra 0 e 255 |

### unhideRow(int row) {#unhideRow-int-}
```
public void unhideRow(int row)
```


Rivela una riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

