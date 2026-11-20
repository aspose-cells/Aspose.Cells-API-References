---
title: "ExportTableOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta tutte le opzioni di esportazione della tabella."
type: docs
url: /it/java/com.aspose.cells/exporttableoptions/
---

**Inheritance:**
java.lang.Object
```
public class ExportTableOptions
```

Rappresenta tutte le opzioni di esportazione della tabella.

**Remarks**

Se ci sono requisiti speciali per l'esportazione, come ignorare i valori di errore, l'utente può estendere questa classe per sovrascrivere le API corrispondenti e raggiungere l'obiettivo.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ExportTableOptions()](#ExportTableOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowDBNull()](#getAllowDBNull--) | Questo valore indica se i DBNull sono consentiti in questa tabella. |
| [getCheckMixedValueType()](#getCheckMixedValueType--) | False, Aspose.Cells imposterà il tipo della DataColumn in base al tipo di valore della prima riga per migliorare le prestazioni. |
| [getClass()](#getClass--) |  |
| [getExportAsHtmlString()](#getExportAsHtmlString--) | Esporta il valore stringa html delle celle nella DataTable. |
| [getExportAsString()](#getExportAsString--) | Esporta il valore stringa delle celle nella DataTable. |
| [getExportColumnName()](#getExportColumnName--) | Indica se i dati nella prima riga vengono esportati nel nome della colonna della DataTable. |
| [getFormatStrategy()](#getFormatStrategy--) | Ottiene la strategia di formattazione quando si esporta il valore come valore stringa. |
| [getIndexes()](#getIndexes--) | Gli indici di colonne/righe che devono essere esportati. |
| [getPlotVisibleCells()](#getPlotVisibleCells--) | Esporta solo le celle visibili. |
| [getPlotVisibleColumns()](#getPlotVisibleColumns--) | Esporta solo le colonne visibili. |
| [getPlotVisibleRows()](#getPlotVisibleRows--) | Esporta solo le righe visibili. |
| [getRenameStrategy()](#getRenameStrategy--) | Strategia per i nomi duplicati delle colonne. |
| [getSkipErrorValue()](#getSkipErrorValue--) | Indica se saltare valori non validi per la colonna. |
| [hashCode()](#hashCode--) |  |
| [isVertical()](#isVertical--) | Vero se una riga nel file Workbook rappresenta una riga nella DataTable. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [preprocessExportedValue(int cellRow, int cellColumn, CellValue value)](#preprocessExportedValue-int-int-com.aspose.cells.CellValue-) | Preelabora il valore della cella corrente da esportare. |
| [setAllowDBNull(boolean value)](#setAllowDBNull-boolean-) | Questo valore indica se i DBNull sono consentiti in questa tabella. |
| [setCheckMixedValueType(boolean value)](#setCheckMixedValueType-boolean-) | False, Aspose.Cells imposterà il tipo della DataColumn in base al tipo di valore della prima riga per migliorare le prestazioni. |
| [setExportAsHtmlString(boolean value)](#setExportAsHtmlString-boolean-) | Esporta il valore stringa html delle celle nella DataTable. |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | Esporta il valore stringa delle celle nella DataTable. |
| [setExportColumnName(boolean value)](#setExportColumnName-boolean-) | Indica se i dati nella prima riga vengono esportati nel nome della colonna della DataTable. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Imposta la strategia di formattazione quando si esporta il valore come stringa. |
| [setIndexes(int[] value)](#setIndexes-int---) | Gli indici di colonne/righe che devono essere esportati. |
| [setPlotVisibleCells(boolean value)](#setPlotVisibleCells-boolean-) | Esporta solo le celle visibili. |
| [setPlotVisibleColumns(boolean value)](#setPlotVisibleColumns-boolean-) | Esporta solo le colonne visibili. |
| [setPlotVisibleRows(boolean value)](#setPlotVisibleRows-boolean-) | Esporta solo le righe visibili. |
| [setRenameStrategy(int value)](#setRenameStrategy-int-) | Strategia per i nomi duplicati delle colonne. |
| [setSkipErrorValue(boolean value)](#setSkipErrorValue-boolean-) | Indica se saltare valori non validi per la colonna. |
| [setVertical(boolean value)](#setVertical-boolean-) | Vero se una riga nel file Workbook rappresenta una riga nella DataTable. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ExportTableOptions() {#ExportTableOptions--}
```
public ExportTableOptions()
```


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
### getAllowDBNull() {#getAllowDBNull--}
```
public boolean getAllowDBNull()
```


Questo valore indica se i DBNull sono consentiti in questa tabella.

**Returns:**
boolean
### getCheckMixedValueType() {#getCheckMixedValueType--}
```
public boolean getCheckMixedValueType()
```


Falso, Aspose.Cells imposterà il tipo della DataColumn's in base al tipo di valore della prima riga per motivi di prestazioni. Vero, Aspose.Cells verificherà se il tipo di valore nella colonna è misto prima di impostare il tipo della DataColumn's e, se i tipi di valore sono misti, il tipo della DataColumn's sarà string.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getExportAsHtmlString() {#getExportAsHtmlString--}
```
public boolean getExportAsHtmlString()
```


Esporta il valore stringa html delle celle nella DataTable.

**Returns:**
boolean
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```


Esporta il valore stringa delle celle nella DataTable.

**Returns:**
boolean
### getExportColumnName() {#getExportColumnName--}
```
public boolean getExportColumnName()
```


Indica se i dati nella prima riga vengono esportati nel nome della colonna della DataTable. Il valore predefinito è false.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Ottiene la strategia di formattazione quando si esporta il valore come valore stringa.

Vedi [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

Il valore predefinito è [CellValueFormatStrategy.CELL\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#CELL-STYLE).

**Returns:**
int
### getIndexes() {#getIndexes--}
```
public int[] getIndexes()
```


Gli indici di colonne/righe che devono essere esportati.

**Returns:**
int[]
### getPlotVisibleCells() {#getPlotVisibleCells--}
```
public boolean getPlotVisibleCells()
```


Esporta solo le celle visibili.

**Returns:**
boolean
### getPlotVisibleColumns() {#getPlotVisibleColumns--}
```
public boolean getPlotVisibleColumns()
```


Esporta solo le colonne visibili.

**Returns:**
boolean
### getPlotVisibleRows() {#getPlotVisibleRows--}
```
public boolean getPlotVisibleRows()
```


Esporta solo le righe visibili.

**Returns:**
boolean
### getRenameStrategy() {#getRenameStrategy--}
```
public int getRenameStrategy()
```


Strategia per i nomi duplicati delle colonne.

Vedi [RenameStrategy](../../com.aspose.cells/renamestrategy).

**Returns:**
int
### getSkipErrorValue() {#getSkipErrorValue--}
```
public boolean getSkipErrorValue()
```


Indica se saltare valori non validi per la colonna. Ad esempio, se il tipo della colonna è decimal, il valore è maggiore di decimal.MaxValue e questa proprietà è true, non verrà sollevata nuovamente un'eccezione. Il valore predefinito è false.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isVertical() {#isVertical--}
```
public boolean isVertical()
```


Vero se una riga nel file Workbook rappresenta una riga nella DataTable. Falso se una colonna nel file Workbook rappresenta una riga nella DataTable.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### preprocessExportedValue(int cellRow, int cellColumn, CellValue value) {#preprocessExportedValue-int-int-com.aspose.cells.CellValue-}
```
public boolean preprocessExportedValue(int cellRow, int cellColumn, CellValue value)
```


Preelabora il valore della cella corrente da esportare.

**Remarks**

L'indice di riga e colonna è l'indice assoluto della cella nel foglio di lavoro, non l'indice nella tabella esportata. L'utente può controllare il valore della cella corrente nell'implementazione di override di questo metodo; se la cella corrente deve essere sostituita con un altro tipo e valore, l'implementazione dovrebbe impostare il tipo e il valore attesi sull'oggetto CellValue e restituire true. Per impostazione predefinita questo metodo non fa nulla e restituisce false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellRow | int | l'indice di riga della cella corrente |
| cellColumn | int | l'indice di colonna della cella |
| value | [CellValue](../../com.aspose.cells/cellvalue) | valore e tipo della cella corrente |

**Returns:**
boolean - Indica se la cella corrente è stata sostituita con un tipo e/o valore diverso.
### setAllowDBNull(boolean value) {#setAllowDBNull-boolean-}
```
public void setAllowDBNull(boolean value)
```


Questo valore indica se i DBNull sono consentiti in questa tabella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCheckMixedValueType(boolean value) {#setCheckMixedValueType-boolean-}
```
public void setCheckMixedValueType(boolean value)
```


Falso, Aspose.Cells imposterà il tipo della DataColumn's in base al tipo di valore della prima riga per motivi di prestazioni. Vero, Aspose.Cells verificherà se il tipo di valore nella colonna è misto prima di impostare il tipo della DataColumn's e, se i tipi di valore sono misti, il tipo della DataColumn's sarà string.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportAsHtmlString(boolean value) {#setExportAsHtmlString-boolean-}
```
public void setExportAsHtmlString(boolean value)
```


Esporta il valore stringa html delle celle nella DataTable.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


Esporta il valore stringa delle celle nella DataTable.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportColumnName(boolean value) {#setExportColumnName-boolean-}
```
public void setExportColumnName(boolean value)
```


Indica se i dati nella prima riga vengono esportati nel nome della colonna della DataTable. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Imposta la strategia di formattazione quando si esporta il valore come stringa.

Vedi [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

Il valore predefinito è [CellValueFormatStrategy.CELL\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#CELL-STYLE).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setIndexes(int[] value) {#setIndexes-int---}
```
public void setIndexes(int[] value)
```


Gli indici di colonne/righe che devono essere esportati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int[] |  |

### setPlotVisibleCells(boolean value) {#setPlotVisibleCells-boolean-}
```
public void setPlotVisibleCells(boolean value)
```


Esporta solo le celle visibili.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPlotVisibleColumns(boolean value) {#setPlotVisibleColumns-boolean-}
```
public void setPlotVisibleColumns(boolean value)
```


Esporta solo le colonne visibili.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPlotVisibleRows(boolean value) {#setPlotVisibleRows-boolean-}
```
public void setPlotVisibleRows(boolean value)
```


Esporta solo le righe visibili.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRenameStrategy(int value) {#setRenameStrategy-int-}
```
public void setRenameStrategy(int value)
```


Strategia per i nomi duplicati delle colonne.

Vedi [RenameStrategy](../../com.aspose.cells/renamestrategy).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSkipErrorValue(boolean value) {#setSkipErrorValue-boolean-}
```
public void setSkipErrorValue(boolean value)
```


Indica se saltare valori non validi per la colonna. Ad esempio, se il tipo della colonna è decimal, il valore è maggiore di decimal.MaxValue e questa proprietà è true, non verrà sollevata nuovamente un'eccezione. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setVertical(boolean value) {#setVertical-boolean-}
```
public void setVertical(boolean value)
```


Vero se una riga nel file Workbook rappresenta una riga nella DataTable. Falso se una colonna nel file Workbook rappresenta una riga nella DataTable.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

