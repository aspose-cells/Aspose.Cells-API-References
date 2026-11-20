---
title: "ImportTableOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni di importazione dei dati nelle celle."
type: docs
url: /it/java/com.aspose.cells/importtableoptions/
---

**Inheritance:**
java.lang.Object
```
public class ImportTableOptions
```

Rappresenta le opzioni di importazione dei dati nelle celle.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ImportTableOptions()](#ImportTableOptions--) | Crea le opzioni di importazione predefinite. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCheckMergedCells()](#getCheckMergedCells--) | Indica se controllare le celle unite. |
| [getClass()](#getClass--) |  |
| [getColumnIndexes()](#getColumnIndexes--) | Ottiene le colonne (indice base 0) da importare dalla fonte dati. null indica che tutte le colonne devono essere importate. |
| [getConvertGridStyle()](#getConvertGridStyle--) | Indica se applicare lo stile della visualizzazione a griglia alle celle. |
| [getConvertNumericData()](#getConvertNumericData--) | Ottiene un valore che indica se il valore stringa deve essere convertito in valore numerico o data. |
| [getDateFormat()](#getDateFormat--) | Ottiene la stringa di formato data per le celle con valori datetime importati. |
| [getDefaultValues()](#getDefaultValues--) | Il valore predefinito per il valore nella tabella è null. |
| [getExportCaptionAsFieldName()](#getExportCaptionAsFieldName--) | Indica se esportare la didascalia come nome campo |
| [getInsertRows()](#getInsertRows--) | Indica se devono essere aggiunte nuove righe per l'importazione dei record dati. |
| [getNumberFormats()](#getNumberFormats--) | Ottiene i formati numerici |
| [getShiftFirstRowDown()](#getShiftFirstRowDown--) | Indica se spostare verso il basso la prima riga durante l'inserimento di righe. |
| [getStyles()](#getStyles--) | Ottiene gli stili per ogni colonna della tabella. |
| [getTotalColumns()](#getTotalColumns--) | Ottiene il conteggio totale delle colonne da importare dalla fonte dati. -1 indica tutte le righe della fonte dati fornita. |
| [getTotalRows()](#getTotalRows--) | Ottiene il conteggio totale delle righe da importare dalla fonte dati. -1 indica tutte le righe della fonte dati fornita. |
| [hashCode()](#hashCode--) |  |
| [isFieldNameShown()](#isFieldNameShown--) | Indica se il nome del campo deve essere importato. |
| [isFormulas()](#isFormulas--) | Indica se i dati sono formule. |
| [isHtmlString()](#isHtmlString--) | Indica se il valore contiene tag html. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCheckMergedCells(boolean value)](#setCheckMergedCells-boolean-) | Indica se controllare le celle unite. |
| [setColumnIndexes(int[] value)](#setColumnIndexes-int---) | Imposta le colonne (indice base 0) da importare dalla fonte dati. null significa che devono essere importate tutte le colonne. |
| [setConvertGridStyle(boolean value)](#setConvertGridStyle-boolean-) | Indica se applicare lo stile della visualizzazione a griglia alle celle. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Imposta un valore che indica se il valore stringa deve essere convertito in valore numerico o data. |
| [setDateFormat(String value)](#setDateFormat-java.lang.String-) | Imposta la stringa di formato data per le celle con valori datetime importati. |
| [setDefaultValues(Object[] value)](#setDefaultValues-java.lang.Object---) | Il valore predefinito per il valore nella tabella è null. |
| [setExportCaptionAsFieldName(boolean value)](#setExportCaptionAsFieldName-boolean-) | Indica se esportare la didascalia come nome campo |
| [setFieldNameShown(boolean value)](#setFieldNameShown-boolean-) | Indica se il nome del campo deve essere importato. |
| [setFormulas(boolean[] value)](#setFormulas-boolean---) | Indica se i dati sono formule. |
| [setHtmlString(boolean value)](#setHtmlString-boolean-) | Indica se il valore contiene tag html. |
| [setInsertRows(boolean value)](#setInsertRows-boolean-) | Indica se devono essere aggiunte nuove righe per l'importazione dei record dati. |
| [setNumberFormats(String[] value)](#setNumberFormats-java.lang.String---) | Imposta i formati numerici |
| [setShiftFirstRowDown(boolean value)](#setShiftFirstRowDown-boolean-) | Indica se spostare verso il basso la prima riga durante l'inserimento di righe. |
| [setStyles(Style[] value)](#setStyles-com.aspose.cells.Style---) | Imposta gli stili per ogni colonna della tabella. |
| [setTotalColumns(int value)](#setTotalColumns-int-) | Imposta il conteggio totale delle colonne da importare dalla fonte dati. -1 significa tutte le righe della fonte dati specificata. |
| [setTotalRows(int value)](#setTotalRows-int-) | Imposta il conteggio totale delle righe da importare dalla fonte dati. -1 significa tutte le righe della fonte dati specificata. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ImportTableOptions() {#ImportTableOptions--}
```
public ImportTableOptions()
```


Crea le opzioni di importazione predefinite.

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
### getCheckMergedCells() {#getCheckMergedCells--}
```
public boolean getCheckMergedCells()
```


Indica se controllare le celle unite.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnIndexes() {#getColumnIndexes--}
```
public int[] getColumnIndexes()
```


Ottiene le colonne (indice base 0) da importare dalla fonte dati. null indica che tutte le colonne devono essere importate.

**Returns:**
int[]
### getConvertGridStyle() {#getConvertGridStyle--}
```
public boolean getConvertGridStyle()
```


Indica se applicare lo stile della visualizzazione a griglia alle celle.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Ottiene un valore che indica se il valore stringa deve essere convertito in valore numerico o data.

**Returns:**
boolean
### getDateFormat() {#getDateFormat--}
```
public String getDateFormat()
```


Ottiene la stringa di formato data per le celle con valori datetime importati.

**Returns:**
java.lang.String
### getDefaultValues() {#getDefaultValues--}
```
public Object[] getDefaultValues()
```


Il valore predefinito per il valore nella tabella è null.

**Returns:**
java.lang.Object[]
### getExportCaptionAsFieldName() {#getExportCaptionAsFieldName--}
```
public boolean getExportCaptionAsFieldName()
```


Indica se esportare la didascalia come nome campo

**Remarks**

Funziona solo per DataTable.

**Returns:**
boolean
### getInsertRows() {#getInsertRows--}
```
public boolean getInsertRows()
```


Indica se devono essere aggiunte nuove righe per l'importazione dei record dati.

**Returns:**
boolean
### getNumberFormats() {#getNumberFormats--}
```
public String[] getNumberFormats()
```


Ottiene i formati numerici

**Returns:**
java.lang.String[]
### getShiftFirstRowDown() {#getShiftFirstRowDown--}
```
public boolean getShiftFirstRowDown()
```


Indica se spostare verso il basso la prima riga durante l'inserimento di righe.

**Returns:**
boolean
### getStyles() {#getStyles--}
```
public Style[] getStyles()
```


Ottiene gli stili per ogni colonna della tabella.

**Returns:**
com.aspose.cells.Style[]
### getTotalColumns() {#getTotalColumns--}
```
public int getTotalColumns()
```


Ottiene il conteggio totale delle colonne da importare dalla fonte dati. -1 indica tutte le righe della fonte dati fornita.

**Returns:**
int
### getTotalRows() {#getTotalRows--}
```
public int getTotalRows()
```


Ottiene il conteggio totale delle righe da importare dalla fonte dati. -1 indica tutte le righe della fonte dati fornita.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFieldNameShown() {#isFieldNameShown--}
```
public boolean isFieldNameShown()
```


Indica se il nome del campo deve essere importato.

**Returns:**
boolean
### isFormulas() {#isFormulas--}
```
public boolean[] isFormulas()
```


Indica se i dati sono formule.

**Returns:**
boolean[]
### isHtmlString() {#isHtmlString--}
```
public boolean isHtmlString()
```


Indica se il valore contiene tag html.

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




### setCheckMergedCells(boolean value) {#setCheckMergedCells-boolean-}
```
public void setCheckMergedCells(boolean value)
```


Indica se controllare le celle unite.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setColumnIndexes(int[] value) {#setColumnIndexes-int---}
```
public void setColumnIndexes(int[] value)
```


Imposta le colonne (indice base 0) da importare dalla fonte dati. null significa che devono essere importate tutte le colonne.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int[] |  |

### setConvertGridStyle(boolean value) {#setConvertGridStyle-boolean-}
```
public void setConvertGridStyle(boolean value)
```


Indica se applicare lo stile della visualizzazione a griglia alle celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Imposta un valore che indica se il valore stringa deve essere convertito in valore numerico o data.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDateFormat(String value) {#setDateFormat-java.lang.String-}
```
public void setDateFormat(String value)
```


Imposta la stringa di formato data per le celle con valori datetime importati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setDefaultValues(Object[] value) {#setDefaultValues-java.lang.Object---}
```
public void setDefaultValues(Object[] value)
```


Il valore predefinito per il valore nella tabella è null.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object[] |  |

### setExportCaptionAsFieldName(boolean value) {#setExportCaptionAsFieldName-boolean-}
```
public void setExportCaptionAsFieldName(boolean value)
```


Indica se esportare la didascalia come nome campo

**Remarks**

Funziona solo per DataTable.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFieldNameShown(boolean value) {#setFieldNameShown-boolean-}
```
public void setFieldNameShown(boolean value)
```


Indica se il nome del campo deve essere importato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFormulas(boolean[] value) {#setFormulas-boolean---}
```
public void setFormulas(boolean[] value)
```


Indica se i dati sono formule.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean[] |  |

### setHtmlString(boolean value) {#setHtmlString-boolean-}
```
public void setHtmlString(boolean value)
```


Indica se il valore contiene tag html.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setInsertRows(boolean value) {#setInsertRows-boolean-}
```
public void setInsertRows(boolean value)
```


Indica se devono essere aggiunte nuove righe per l'importazione dei record dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setNumberFormats(String[] value) {#setNumberFormats-java.lang.String---}
```
public void setNumberFormats(String[] value)
```


Imposta i formati numerici

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String[] |  |

### setShiftFirstRowDown(boolean value) {#setShiftFirstRowDown-boolean-}
```
public void setShiftFirstRowDown(boolean value)
```


Indica se spostare verso il basso la prima riga durante l'inserimento di righe.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setStyles(Style[] value) {#setStyles-com.aspose.cells.Style---}
```
public void setStyles(Style[] value)
```


Imposta gli stili per ogni colonna della tabella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Style\[\]](../../com.aspose.cells/style) |  |

### setTotalColumns(int value) {#setTotalColumns-int-}
```
public void setTotalColumns(int value)
```


Imposta il conteggio totale delle colonne da importare dalla fonte dati. -1 significa tutte le righe della fonte dati specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTotalRows(int value) {#setTotalRows-int-}
```
public void setTotalRows(int value)
```


Imposta il conteggio totale delle righe da importare dalla fonte dati. -1 significa tutte le righe della fonte dati specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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

