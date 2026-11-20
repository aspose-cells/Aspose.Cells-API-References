---
title: "TxtSaveOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni di salvataggio per il formato csv/tab delimitato/altri formati di testo."
type: docs
url: /it/java/com.aspose.cells/txtsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class TxtSaveOptions extends SaveOptions
```

Rappresenta le opzioni di salvataggio per il formato csv/tab delimitato/altri formati di testo.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [TxtSaveOptions()](#TxtSaveOptions--) | Crea le opzioni di salvataggio per file di testo. |
| [TxtSaveOptions(int saveFormat)](#TxtSaveOptions-int-) | Crea le opzioni di salvataggio per file di testo. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlwaysQuoted()](#getAlwaysQuoted--) | Indica se aggiungere sempre \" per ogni campo. |
| [getCachedFileFolder()](#getCachedFileFolder--) | La cartella per i file temporanei che possono essere usati come cache dei dati. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Rendi il workbook vuoto dopo aver salvato il file. |
| [getCreateDirectory()](#getCreateDirectory--) | Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [getEncoding()](#getEncoding--) | Ottiene la codifica predefinita. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indica se crittografare le proprietà del documento quando si salva come file .xls. |
| [getExportAllSheets()](#getExportAllSheets--) | Indica se esportare tutti i fogli nel file di testo. |
| [getExportArea()](#getExportArea--) | L'intervallo di celle da esportare. |
| [getExportQuotePrefix()](#getExportQuotePrefix--) | Indica se il segno di apice singolo deve essere esportato come parte del valore di una cella quando [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) è vero per essa. |
| [getFormatStrategy()](#getFormatStrategy--) | Ottiene la strategia di formattazione quando si esporta il valore della cella come stringa. |
| [getKeepSeparatorsForBlankRow()](#getKeepSeparatorsForBlankRow--) | Indica se i separatori devono essere emessi per le righe vuote. |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | Il provider di dati per salvare la cartella di lavoro in modalità leggera. |
| [getMergeAreas()](#getMergeAreas--) | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. |
| [getQuoteType()](#getQuoteType--) | Ottiene come citare i valori nel file di testo esportato. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indica se memorizzare nella cache i dati più recenti del grafico. |
| [getSaveFormat()](#getSaveFormat--) | Ottiene il formato di salvataggio del file. |
| [getSeparator()](#getSeparator--) | Ottiene il delimitatore di carattere del file di testo. |
| [getSeparatorString()](#getSeparatorString--) | Ottiene un valore stringa come separatore. |
| [getSortExternalNames()](#getSortExternalNames--) | Indica se ordinare i nomi definiti esterni prima di salvare il file. |
| [getSortNames()](#getSortNames--) | Indica se ordinare i nomi definiti prima di salvare il file. |
| [getTrimLeadingBlankRowAndColumn()](#getTrimLeadingBlankRowAndColumn--) | Indica se le righe e le colonne vuote iniziali devono essere eliminate come fa ms excel. |
| [getTrimTailingBlankCells()](#getTrimTailingBlankCells--) | Indica se le celle vuote finali in una riga devono essere eliminate. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indica se aggiornare le impostazioni di SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indica se convalidare le celle unite prima di salvare il file. |
| [getWarningCallback()](#getWarningCallback--) | Ottiene il callback di avviso. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlwaysQuoted(boolean value)](#setAlwaysQuoted-boolean-) | Indica se aggiungere sempre \" per ogni campo. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | La cartella per i file temporanei che possono essere usati come cache dei dati. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [setClearData(boolean value)](#setClearData-boolean-) | Rendi il workbook vuoto dopo aver salvato il file. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Imposta la codifica predefinita. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indica se crittografare le proprietà del documento quando si salva come file .xls. |
| [setExportAllSheets(boolean value)](#setExportAllSheets-boolean-) | Indica se esportare tutti i fogli nel file di testo. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | L'intervallo di celle da esportare. |
| [setExportQuotePrefix(boolean value)](#setExportQuotePrefix-boolean-) | Indica se il segno di apice singolo deve essere esportato come parte del valore di una cella quando [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) è vero per essa. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Imposta la strategia di formattazione quando si esporta il valore della cella come stringa. |
| [setKeepSeparatorsForBlankRow(boolean value)](#setKeepSeparatorsForBlankRow-boolean-) | Indica se i separatori devono essere emessi per le righe vuote. |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | Il provider di dati per salvare la cartella di lavoro in modalità leggera. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. |
| [setQuoteType(int value)](#setQuoteType-int-) | Imposta come citare i valori nel file di testo esportato. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indica se memorizzare nella cache i dati più recenti del grafico. |
| [setSeparator(char value)](#setSeparator-char-) | Imposta il delimitatore di carattere del file di testo. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Imposta un valore stringa come separatore. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indica se ordinare i nomi definiti esterni prima di salvare il file. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indica se ordinare i nomi definiti prima di salvare il file. |
| [setTrimLeadingBlankRowAndColumn(boolean value)](#setTrimLeadingBlankRowAndColumn-boolean-) | Indica se le righe e le colonne vuote iniziali devono essere eliminate come fa ms excel. |
| [setTrimTailingBlankCells(boolean value)](#setTrimTailingBlankCells-boolean-) | Indica se le celle vuote finali in una riga devono essere eliminate. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indica se aggiornare le impostazioni di SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indica se convalidare le celle unite prima di salvare il file. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Imposta la callback di avviso. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TxtSaveOptions() {#TxtSaveOptions--}
```
public TxtSaveOptions()
```


Crea le opzioni di salvataggio per file di testo.

### TxtSaveOptions(int saveFormat) {#TxtSaveOptions-int-}
```
public TxtSaveOptions(int saveFormat)
```


Crea le opzioni di salvataggio per file di testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Il formato del file. Dovrebbe essere [SaveFormat.CSV](../../com.aspose.cells/saveformat\#CSV) o [SaveFormat.TSV](../../com.aspose.cells/saveformat\#TSV), altrimenti il formato salvato sarà impostato automaticamente su [SaveFormat.CSV](../../com.aspose.cells/saveformat\#CSV). |

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
### getAlwaysQuoted() {#getAlwaysQuoted--}
```
public boolean getAlwaysQuoted()
```


Indica se aggiungere sempre \" per ogni campo. Se vero, tutti i valori saranno citati; se falso, i valori saranno citati solo quando necessario (ad esempio, quando contengono caratteri speciali come \", \\n o il carattere separatore). Il valore predefinito è false.

**Remarks**

NOTE: Questo membro è ora obsoleto. Invece, si prega di usare la proprietà QuoteType. Questa proprietà sarà rimossa tra 12 mesi a partire da agosto 2012. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

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
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Ottiene la codifica predefinita.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Indica se crittografare le proprietà del documento durante il salvataggio come file .xls. Il valore predefinito è true.

**Remarks**

Solo per i file .xls, .xlsx, .xlsb e .xlsm.

**Returns:**
boolean
### getExportAllSheets() {#getExportAllSheets--}
```
public boolean getExportAllSheets()
```


Indica se esportare tutti i fogli nel file di testo. Se è false, esporta solo il foglio attivo, proprio come MS Excel.

**Remarks**

Il valore predefinito è false.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


L'intervallo di celle da esportare.

**Remarks**

Se l'area esportata è stata specificata, [getTrimLeadingBlankRowAndColumn()](../../com.aspose.cells/txtsaveoptions\#getTrimLeadingBlankRowAndColumn--) non avrà alcun effetto.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportQuotePrefix() {#getExportQuotePrefix--}
```
public boolean getExportQuotePrefix()
```


Indica se il segno di apice singolo deve essere esportato come parte del valore di una cella quando [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) è true per essa. Il valore predefinito è false.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Ottiene la strategia di formattazione quando si esporta il valore della cella come stringa.

Vedi [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Returns:**
int
### getKeepSeparatorsForBlankRow() {#getKeepSeparatorsForBlankRow--}
```
public boolean getKeepSeparatorsForBlankRow()
```


Indica se i separatori devono essere emessi per una riga vuota. Il valore predefinito è false, quindi per impostazione predefinita il contenuto della riga vuota sarà vuoto.

**Returns:**
boolean
### getLightCellsDataProvider() {#getLightCellsDataProvider--}
```
public LightCellsDataProvider getLightCellsDataProvider()
```


Il provider di dati per salvare la cartella di lavoro in modalità leggera.

**Returns:**
[LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider)
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file.

**Remarks**

Il valore predefinito è false.

**Returns:**
boolean
### getQuoteType() {#getQuoteType--}
```
public int getQuoteType()
```


Ottiene come citare i valori nel file di testo esportato.

Vedi [TxtValueQuoteType](../../com.aspose.cells/txtvaluequotetype).

**Returns:**
int
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
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Ottiene il delimitatore di carattere del file di testo.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


Ottiene un valore stringa come separatore.

**Returns:**
java.lang.String
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
### getTrimLeadingBlankRowAndColumn() {#getTrimLeadingBlankRowAndColumn--}
```
public boolean getTrimLeadingBlankRowAndColumn()
```


Indica se le righe e le colonne vuote iniziali devono essere eliminate come fa MS Excel. Il valore predefinito è true.

**Remarks**

Stessa regola di MS Excel, una riga/colonna non sarà considerata vuota se ha uno stile personalizzato, anche se non contiene dati di cella. Quando si salva in modalità LightCells, questa opzione non ha effetto. L'utente dovrebbe controllare l'intervallo di output mediante l'implementazione di [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) o specificando [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--)

**Returns:**
boolean
### getTrimTailingBlankCells() {#getTrimTailingBlankCells--}
```
public boolean getTrimTailingBlankCells()
```


Indica se le celle vuote finali in una riga devono essere eliminate. Il valore predefinito è false.

**Remarks**

Quando si salva in modalità LightCells e [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--) non è stato specificato, questa opzione non ha effetto e una riga sarà estesa fino all'ultima cella fornita dall'implementazione [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--)

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




### setAlwaysQuoted(boolean value) {#setAlwaysQuoted-boolean-}
```
public void setAlwaysQuoted(boolean value)
```


Indica se aggiungere sempre \" per ogni campo. Se vero, tutti i valori saranno citati; se falso, i valori saranno citati solo quando necessario (ad esempio, quando contengono caratteri speciali come \", \\n o il carattere separatore). Il valore predefinito è false.

**Remarks**

NOTE: Questo membro è ora obsoleto. Invece, si prega di usare la proprietà QuoteType. Questa proprietà sarà rimossa tra 12 mesi a partire da agosto 2012. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

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

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Imposta la codifica predefinita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

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

### setExportAllSheets(boolean value) {#setExportAllSheets-boolean-}
```
public void setExportAllSheets(boolean value)
```


Indica se esportare tutti i fogli nel file di testo. Se è false, esporta solo il foglio attivo, proprio come MS Excel.

**Remarks**

Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


L'intervallo di celle da esportare.

**Remarks**

Se l'area esportata è stata specificata, [getTrimLeadingBlankRowAndColumn()](../../com.aspose.cells/txtsaveoptions\#getTrimLeadingBlankRowAndColumn--) non avrà alcun effetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportQuotePrefix(boolean value) {#setExportQuotePrefix-boolean-}
```
public void setExportQuotePrefix(boolean value)
```


Indica se il segno di apice singolo deve essere esportato come parte del valore di una cella quando [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) è true per essa. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Imposta la strategia di formattazione quando si esporta il valore della cella come stringa.

Vedi [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setKeepSeparatorsForBlankRow(boolean value) {#setKeepSeparatorsForBlankRow-boolean-}
```
public void setKeepSeparatorsForBlankRow(boolean value)
```


Indica se i separatori devono essere emessi per una riga vuota. Il valore predefinito è false, quindi per impostazione predefinita il contenuto della riga vuota sarà vuoto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLightCellsDataProvider(LightCellsDataProvider value) {#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-}
```
public void setLightCellsDataProvider(LightCellsDataProvider value)
```


Il provider di dati per salvare la cartella di lavoro in modalità leggera.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider) |  |

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

### setQuoteType(int value) {#setQuoteType-int-}
```
public void setQuoteType(int value)
```


Imposta come citare i valori nel file di testo esportato.

Vedi [TxtValueQuoteType](../../com.aspose.cells/txtvaluequotetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Indica se memorizzare nella cache i dati più recenti del grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


Imposta il delimitatore di carattere del file di testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | char |  |

### setSeparatorString(String value) {#setSeparatorString-java.lang.String-}
```
public void setSeparatorString(String value)
```


Imposta un valore stringa come separatore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

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

### setTrimLeadingBlankRowAndColumn(boolean value) {#setTrimLeadingBlankRowAndColumn-boolean-}
```
public void setTrimLeadingBlankRowAndColumn(boolean value)
```


Indica se le righe e le colonne vuote iniziali devono essere eliminate come fa MS Excel. Il valore predefinito è true.

**Remarks**

Stessa regola di MS Excel, una riga/colonna non sarà considerata vuota se ha uno stile personalizzato, anche se non contiene dati di cella. Quando si salva in modalità LightCells, questa opzione non ha effetto. L'utente dovrebbe controllare l'intervallo di output mediante l'implementazione di [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) o specificando [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--)

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setTrimTailingBlankCells(boolean value) {#setTrimTailingBlankCells-boolean-}
```
public void setTrimTailingBlankCells(boolean value)
```


Indica se le celle vuote finali in una riga devono essere eliminate. Il valore predefinito è false.

**Remarks**

Quando si salva in modalità LightCells e [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--) non è stato specificato, questa opzione non ha effetto e una riga sarà estesa fino all'ultima cella fornita dall'implementazione [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--)

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

