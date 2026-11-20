---
title: "JsonSaveOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni per salvare la cartella di lavoro come file JSON."
type: docs
url: /it/java/com.aspose.cells/jsonsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class JsonSaveOptions extends SaveOptions
```

Rappresenta le opzioni per salvare la cartella di lavoro come file JSON.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [JsonSaveOptions()](#JsonSaveOptions--) | Crea opzioni per salvare il file json. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlwaysExportAsJsonObject()](#getAlwaysExportAsJsonObject--) | Indica se esportare sempre Excel in json come oggetto, anche quando c'è solo un foglio di lavoro nel file. |
| [getCachedFileFolder()](#getCachedFileFolder--) | La cartella per i file temporanei che possono essere usati come cache dei dati. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Rendi il workbook vuoto dopo aver salvato il file. |
| [getCreateDirectory()](#getCreateDirectory--) | Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indica se crittografare le proprietà del documento quando si salva come file .xls. |
| [getExportArea()](#getExportArea--) | Ottiene l'intervallo di esportazione. |
| [getExportAsString()](#getExportAsString--) | Esporta il valore stringa delle celle in json. |
| [getExportEmptyCells()](#getExportEmptyCells--) | Indica se esportare le celle vuote come null. |
| [getExportHyperlinkType()](#getExportHyperlinkType--) | Rappresenta il tipo di esportazione del collegamento ipertestuale in json. |
| [getExportNestedStructure()](#getExportNestedStructure--) | Esportato come struttura Json gerarchica padre-figlio. |
| [getExportStylePool()](#getExportStylePool--) | Indica se esportare gli stili collettivamente o individualmente per ogni cella. |
| [getIndent()](#getIndent--) | Indica l'indentazione. |
| [getMergeAreas()](#getMergeAreas--) | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indica se memorizzare nella cache i dati più recenti del grafico. |
| [getSaveFormat()](#getSaveFormat--) | Ottiene il formato di salvataggio del file. |
| [getSchemas()](#getSchemas--) | Lo schema json originale di ogni foglio di lavoro. |
| [getSheetIndexes()](#getSheetIndexes--) | Rappresenta gli indici dei fogli esportati. |
| [getSkipEmptyRows()](#getSkipEmptyRows--) | Indica se saltare le righe vuote. |
| [getSortExternalNames()](#getSortExternalNames--) | Indica se ordinare i nomi definiti esterni prima di salvare il file. |
| [getSortNames()](#getSortNames--) | Indica se ordinare i nomi definiti prima di salvare il file. |
| [getToExcelStruct()](#getToExcelStruct--) | Indica se convertire la struttura json del file Excel. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indica se aggiornare le impostazioni di SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indica se convalidare le celle unite prima di salvare il file. |
| [getWarningCallback()](#getWarningCallback--) | Ottiene il callback di avviso. |
| [hasHeaderRow()](#hasHeaderRow--) | Indica se l'intervallo contiene la riga di intestazione. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlwaysExportAsJsonObject(boolean value)](#setAlwaysExportAsJsonObject-boolean-) | Indica se esportare sempre Excel in json come oggetto, anche quando c'è solo un foglio di lavoro nel file. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | La cartella per i file temporanei che possono essere usati come cache dei dati. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [setClearData(boolean value)](#setClearData-boolean-) | Rendi il workbook vuoto dopo aver salvato il file. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indica se crittografare le proprietà del documento quando si salva come file .xls. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Imposta l'intervallo di esportazione. |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | Esporta il valore stringa delle celle in json. |
| [setExportEmptyCells(boolean value)](#setExportEmptyCells-boolean-) | Indica se esportare le celle vuote come null. |
| [setExportHyperlinkType(int value)](#setExportHyperlinkType-int-) | Rappresenta il tipo di esportazione del collegamento ipertestuale in json. |
| [setExportNestedStructure(boolean value)](#setExportNestedStructure-boolean-) | Esportato come struttura Json gerarchica padre-figlio. |
| [setExportStylePool(boolean value)](#setExportStylePool-boolean-) | Indica se esportare gli stili collettivamente o individualmente per ogni cella. |
| [setHasHeaderRow(boolean value)](#setHasHeaderRow-boolean-) | Indica se l'intervallo contiene la riga di intestazione. |
| [setIndent(String value)](#setIndent-java.lang.String-) | Indica l'indentazione. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indica se memorizzare nella cache i dati più recenti del grafico. |
| [setSchemas(String[] value)](#setSchemas-java.lang.String---) | Lo schema json originale di ogni foglio di lavoro. |
| [setSheetIndexes(int[] value)](#setSheetIndexes-int---) | Rappresenta gli indici dei fogli esportati. |
| [setSkipEmptyRows(boolean value)](#setSkipEmptyRows-boolean-) | Indica se saltare le righe vuote. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indica se ordinare i nomi definiti esterni prima di salvare il file. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indica se ordinare i nomi definiti prima di salvare il file. |
| [setToExcelStruct(boolean value)](#setToExcelStruct-boolean-) | Indica se convertire la struttura json del file Excel. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indica se aggiornare le impostazioni di SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indica se convalidare le celle unite prima di salvare il file. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Imposta la callback di avviso. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### JsonSaveOptions() {#JsonSaveOptions--}
```
public JsonSaveOptions()
```


Crea opzioni per salvare il file json.

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
### getAlwaysExportAsJsonObject() {#getAlwaysExportAsJsonObject--}
```
public boolean getAlwaysExportAsJsonObject()
```


Indica se esportare sempre Excel in json come oggetto, anche quando c'è solo un foglio di lavoro nel file.

**Returns:**
boolean
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


La cartella per i file temporanei che possono essere usati come cache dei dati.

**Remarks**

Se la cartella non è stata specificata, il valore predefinito è [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Se il suo valore predefinito è null o vuoto, o è stato specificato come null o vuoto, allora non verrà utilizzato alcun file di cache durante il salvataggio del workbook.

**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Ad esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando si inserisce un valore più lungo di 32K, verrà troncato.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


Rendi il workbook vuoto dopo aver salvato il file.

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file.

**Remarks**

Il valore predefinito è false.

**Returns:**
boolean
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Indica se crittografare le proprietà del documento durante il salvataggio come file .xls. Il valore predefinito è true.

**Remarks**

Solo per i file .xls, .xlsx, .xlsb e .xlsm.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


Ottiene l'intervallo di esportazione.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```


Esporta il valore stringa delle celle in json.

**Returns:**
boolean
### getExportEmptyCells() {#getExportEmptyCells--}
```
public boolean getExportEmptyCells()
```


Indica se esportare le celle vuote come null.

**Returns:**
boolean
### getExportHyperlinkType() {#getExportHyperlinkType--}
```
public int getExportHyperlinkType()
```


Rappresenta il tipo di esportazione del collegamento ipertestuale in json.

Vedi [JsonExportHyperlinkType](../../com.aspose.cells/jsonexporthyperlinktype).

**Remarks**

Il valore predefinito è [JsonExportHyperlinkType.DISPLAY\\_STRING](../../com.aspose.cells/jsonexporthyperlinktype\\#DISPLAY-STRING);

**Returns:**
int
### getExportNestedStructure() {#getExportNestedStructure--}
```
public boolean getExportNestedStructure()
```


Esportato come struttura Json gerarchica padre-figlio.

**Remarks**

**Returns:**
boolean
### getExportStylePool() {#getExportStylePool--}
```
public boolean getExportStylePool()
```


Indica se esportare gli stili collettivamente o individualmente per ogni cella.

**Returns:**
boolean
### getIndent() {#getIndent--}
```
public String getIndent()
```


Indica l'indentazione.

**Remarks**

Se l'indentazione è nulla o vuota, il JSON esportato non è formattato.

**Returns:**
java.lang.String
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file.

**Remarks**

Il valore predefinito è false.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Indica se memorizzare nella cache i dati più recenti del grafico.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Ottiene il formato di salvataggio del file.

Vedi [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSchemas() {#getSchemas--}
```
public String[] getSchemas()
```


Lo schema json originale di ogni foglio di lavoro.

**Returns:**
java.lang.String[]
### getSheetIndexes() {#getSheetIndexes--}
```
public int[] getSheetIndexes()
```


Rappresenta gli indici dei fogli esportati.

**Returns:**
int[]
### getSkipEmptyRows() {#getSkipEmptyRows--}
```
public boolean getSkipEmptyRows()
```


Indica se saltare le righe vuote.

**Returns:**
boolean
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


Indica se ordinare i nomi definiti esterni prima di salvare il file.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Indica se ordinare i nomi definiti prima di salvare il file.

**Returns:**
boolean
### getToExcelStruct() {#getToExcelStruct--}
```
public boolean getToExcelStruct()
```


Indica se convertire la struttura json del file Excel.

**Remarks**

Solo per la conversione dell'intervallo in JSON.

**Returns:**
boolean
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Indica se aggiornare l'impostazione Smart Art. Il valore predefinito è false.

**Remarks**

Ha effetto solo dopo aver chiamato il metodo Shape.GetResultOfSmartArt() e quando le forme memorizzate nella cache esistono nel file modello.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Indica se convalidare le celle unite prima di salvare il file.

**Remarks**

Il valore predefinito è false.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Ottiene il callback di avviso.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hasHeaderRow() {#hasHeaderRow--}
```
public boolean hasHeaderRow()
```


Indica se l'intervallo contiene la riga di intestazione.

**Returns:**
boolean
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




### setAlwaysExportAsJsonObject(boolean value) {#setAlwaysExportAsJsonObject-boolean-}
```
public void setAlwaysExportAsJsonObject(boolean value)
```


Indica se esportare sempre Excel in json come oggetto, anche quando c'è solo un foglio di lavoro nel file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


La cartella per i file temporanei che possono essere usati come cache dei dati.

**Remarks**

Se la cartella non è stata specificata, il valore predefinito è [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Se il suo valore predefinito è null o vuoto, o è stato specificato come null o vuoto, allora non verrà utilizzato alcun file di cache durante il salvataggio del workbook.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Ad esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando si inserisce un valore più lungo di 32K, verrà troncato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Rendi il workbook vuoto dopo aver salvato il file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file.

**Remarks**

Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


Indica se crittografare le proprietà del documento durante il salvataggio come file .xls. Il valore predefinito è true.

**Remarks**

Solo per i file .xls, .xlsx, .xlsb e .xlsm.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


Imposta l'intervallo di esportazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


Esporta il valore stringa delle celle in json.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportEmptyCells(boolean value) {#setExportEmptyCells-boolean-}
```
public void setExportEmptyCells(boolean value)
```


Indica se esportare le celle vuote come null.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportHyperlinkType(int value) {#setExportHyperlinkType-int-}
```
public void setExportHyperlinkType(int value)
```


Rappresenta il tipo di esportazione del collegamento ipertestuale in json.

Vedi [JsonExportHyperlinkType](../../com.aspose.cells/jsonexporthyperlinktype).

**Remarks**

Il valore predefinito è [JsonExportHyperlinkType.DISPLAY\\_STRING](../../com.aspose.cells/jsonexporthyperlinktype\\#DISPLAY-STRING);

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setExportNestedStructure(boolean value) {#setExportNestedStructure-boolean-}
```
public void setExportNestedStructure(boolean value)
```


Esportato come struttura Json gerarchica padre-figlio.

**Remarks**

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportStylePool(boolean value) {#setExportStylePool-boolean-}
```
public void setExportStylePool(boolean value)
```


Indica se esportare gli stili collettivamente o individualmente per ogni cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHasHeaderRow(boolean value) {#setHasHeaderRow-boolean-}
```
public void setHasHeaderRow(boolean value)
```


Indica se l'intervallo contiene la riga di intestazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setIndent(String value) {#setIndent-java.lang.String-}
```
public void setIndent(String value)
```


Indica l'indentazione.

**Remarks**

Se l'indentazione è nulla o vuota, il JSON esportato non è formattato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file.

**Remarks**

Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Indica se memorizzare nella cache i dati più recenti del grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSchemas(String[] value) {#setSchemas-java.lang.String---}
```
public void setSchemas(String[] value)
```


Lo schema json originale di ogni foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String[] |  |

### setSheetIndexes(int[] value) {#setSheetIndexes-int---}
```
public void setSheetIndexes(int[] value)
```


Rappresenta gli indici dei fogli esportati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int[] |  |

### setSkipEmptyRows(boolean value) {#setSkipEmptyRows-boolean-}
```
public void setSkipEmptyRows(boolean value)
```


Indica se saltare le righe vuote.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


Indica se ordinare i nomi definiti esterni prima di salvare il file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Indica se ordinare i nomi definiti prima di salvare il file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setToExcelStruct(boolean value) {#setToExcelStruct-boolean-}
```
public void setToExcelStruct(boolean value)
```


Indica se convertire la struttura json del file Excel.

**Remarks**

Solo per la conversione dell'intervallo in JSON.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


Indica se aggiornare l'impostazione Smart Art. Il valore predefinito è false.

**Remarks**

Ha effetto solo dopo aver chiamato il metodo Shape.GetResultOfSmartArt() e quando le forme memorizzate nella cache esistono nel file modello.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Indica se convalidare le celle unite prima di salvare il file.

**Remarks**

Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Imposta la callback di avviso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

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

