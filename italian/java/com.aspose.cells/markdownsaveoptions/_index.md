---
title: "MarkdownSaveOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni di salvataggio per markdown."
type: docs
url: /it/java/com.aspose.cells/markdownsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class MarkdownSaveOptions extends SaveOptions
```

Rappresenta le opzioni di salvataggio per markdown.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [MarkdownSaveOptions()](#MarkdownSaveOptions--) | Crea le opzioni per salvare il documento markdown |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlignColumnPadding()](#getAlignColumnPadding--) | Indica se l'allineamento delle colonne è abilitato per le tabelle Markdown generate. |
| [getCachedFileFolder()](#getCachedFileFolder--) | La cartella per i file temporanei che possono essere usati come cache dei dati. |
| [getCalculateFormula()](#getCalculateFormula--) | Indica se calcolare le formule prima di salvare il file markdown. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Rendi il workbook vuoto dopo aver salvato il file. |
| [getCreateDirectory()](#getCreateDirectory--) | Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [getEncoding()](#getEncoding--) | Ottiene la codifica predefinita. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indica se crittografare le proprietà del documento quando si salva come file .xls. |
| [getExportHyperlinkAsReference()](#getExportHyperlinkAsReference--) | Indica se esportare i collegamenti ipertestuali usando definizioni di riferimento invece del formato inline. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | Specifica se le immagini vengono salvate in formato Base64 nel Markdown. |
| [getFormatStrategy()](#getFormatStrategy--) | Ottiene la strategia di formattazione quando si esporta il valore della cella come stringa. |
| [getImageOptions()](#getImageOptions--) | Ottieni l'oggetto ImageOrPrintOptions prima dell'esportazione |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | Il provider di dati per fornire i dati delle celle durante il salvataggio della cartella di lavoro in modalità leggera. |
| [getLineSeparator()](#getLineSeparator--) | Ottiene il separatore di riga. |
| [getMergeAreas()](#getMergeAreas--) | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. |
| [getOfficeMathOutputType()](#getOfficeMathOutputType--) | Indica come gli oggetti OfficeMath vengono esportati in Markdown, il valore predefinito è Immagine. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indica se memorizzare nella cache i dati più recenti del grafico. |
| [getSaveFormat()](#getSaveFormat--) | Ottiene il formato di salvataggio del file. |
| [getSheetSet()](#getSheetSet--) | Ottiene i fogli da renderizzare. |
| [getSortExternalNames()](#getSortExternalNames--) | Indica se ordinare i nomi definiti esterni prima di salvare il file. |
| [getSortNames()](#getSortNames--) | Indica se ordinare i nomi definiti prima di salvare il file. |
| [getSplitTablesByBlankRow()](#getSplitTablesByBlankRow--) | Indica se le righe vuote nel foglio di lavoro devono essere trattate come separatori di tabella durante l'esportazione in Markdown. |
| [getStreamProvider()](#getStreamProvider--) | Ottiene l'IStreamProvider per l'esportazione degli oggetti. |
| [getTableHeaderType()](#getTableHeaderType--) | Ottiene come impostare l'intestazione della tabella. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indica se aggiornare le impostazioni di SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indica se convalidare le celle unite prima di salvare il file. |
| [getWarningCallback()](#getWarningCallback--) | Ottiene il callback di avviso. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignColumnPadding(char value)](#setAlignColumnPadding-char-) | Indica se l'allineamento delle colonne è abilitato per le tabelle Markdown generate. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | La cartella per i file temporanei che possono essere usati come cache dei dati. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Indica se calcolare le formule prima di salvare il file markdown. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [setClearData(boolean value)](#setClearData-boolean-) | Rendi il workbook vuoto dopo aver salvato il file. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Imposta la codifica predefinita. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indica se crittografare le proprietà del documento quando si salva come file .xls. |
| [setExportHyperlinkAsReference(boolean value)](#setExportHyperlinkAsReference-boolean-) | Indica se esportare i collegamenti ipertestuali usando definizioni di riferimento invece del formato inline. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | Specifica se le immagini vengono salvate in formato Base64 nel Markdown. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Imposta la strategia di formattazione quando si esporta il valore della cella come stringa. |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | Il provider di dati per fornire i dati delle celle durante il salvataggio della cartella di lavoro in modalità leggera. |
| [setLineSeparator(String value)](#setLineSeparator-java.lang.String-) | Imposta il separatore di riga. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. |
| [setOfficeMathOutputType(int value)](#setOfficeMathOutputType-int-) | Indica come gli oggetti OfficeMath vengono esportati in Markdown, il valore predefinito è Immagine. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indica se memorizzare nella cache i dati più recenti del grafico. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Imposta i fogli da rendere. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indica se ordinare i nomi definiti esterni prima di salvare il file. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indica se ordinare i nomi definiti prima di salvare il file. |
| [setSplitTablesByBlankRow(boolean value)](#setSplitTablesByBlankRow-boolean-) | Indica se le righe vuote nel foglio di lavoro devono essere trattate come separatori di tabella durante l'esportazione in Markdown. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Imposta l'IStreamProvider per l'esportazione degli oggetti. |
| [setTableHeaderType(int value)](#setTableHeaderType-int-) | Imposta come impostare l'intestazione della tabella. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indica se aggiornare le impostazioni di SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indica se convalidare le celle unite prima di salvare il file. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Imposta la callback di avviso. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### MarkdownSaveOptions() {#MarkdownSaveOptions--}
```
public MarkdownSaveOptions()
```


Crea le opzioni per salvare il documento markdown

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
### getAlignColumnPadding() {#getAlignColumnPadding--}
```
public char getAlignColumnPadding()
```


Indica se l'allineamento delle colonne è abilitato per le tabelle Markdown generate. Quando abilitato, le colonne sono allineate aggiungendo spazi al contenuto delle celle con il carattere specificato (tipicamente ' ' per gli spazi). Impostare a '\\0' per disabilitare l'allineamento delle colonne (predefinito).

**Returns:**
char
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


La cartella per i file temporanei che possono essere usati come cache dei dati.

**Remarks**

Se la cartella non è stata specificata, il valore predefinito è [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Se il suo valore predefinito è null o vuoto, o è stato specificato come null o vuoto, allora non verrà utilizzato alcun file di cache durante il salvataggio del workbook.

**Returns:**
java.lang.String
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


Indica se calcolare le formule prima di salvare il file markdown.

**Remarks**

Il valore predefinito è false.

**Returns:**
boolean
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
### getExportHyperlinkAsReference() {#getExportHyperlinkAsReference--}
```
public boolean getExportHyperlinkAsReference()
```


Indica se esportare i collegamenti ipertestuali usando definizioni di riferimento invece del formato inline. Il valore predefinito è false.

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


Specifica se le immagini vengono salvate in formato Base64 nel Markdown. Il valore predefinito è true.

**Remarks**

Quando questa proprietà è impostata su true, i dati dell'immagine vengono esportati direttamente negli elementi img e non vengono creati file separati.

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
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


Ottieni l'oggetto ImageOrPrintOptions prima dell'esportazione

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
### getLightCellsDataProvider() {#getLightCellsDataProvider--}
```
public LightCellsDataProvider getLightCellsDataProvider()
```


Il provider di dati per fornire i dati delle celle durante il salvataggio della cartella di lavoro in modalità leggera.

**Returns:**
[LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider)
### getLineSeparator() {#getLineSeparator--}
```
public String getLineSeparator()
```


Ottiene il separatore di riga.

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
### getOfficeMathOutputType() {#getOfficeMathOutputType--}
```
public int getOfficeMathOutputType()
```


Indica come gli oggetti OfficeMath vengono esportati in Markdown, il valore predefinito è Immagine.

Vedi [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

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
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Ottiene i fogli da renderizzare. Il valore predefinito è tutti i fogli visibili nella cartella di lavoro: [SheetSet.getActive()](../../com.aspose.cells/sheetset\#getActive--).

**Remarks**

Il set è ignorato quando viene utilizzato in [SheetRender](../../com.aspose.cells/sheetrender)

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
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
### getSplitTablesByBlankRow() {#getSplitTablesByBlankRow--}
```
public boolean getSplitTablesByBlankRow()
```


Indica se le righe vuote nel foglio di lavoro devono essere trattate come separatori di tabella durante l'esportazione in Markdown. Il valore predefinito è false.

**Returns:**
boolean
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Ottiene l'IStreamProvider per l'esportazione degli oggetti. Se `null`, gli oggetti esportati saranno salvati nella stessa directory del file di output.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getTableHeaderType() {#getTableHeaderType--}
```
public int getTableHeaderType()
```


Ottiene come impostare l'intestazione della tabella.

Vedi [MarkdownTableHeaderType](../../com.aspose.cells/markdowntableheadertype).

**Returns:**
int
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




### setAlignColumnPadding(char value) {#setAlignColumnPadding-char-}
```
public void setAlignColumnPadding(char value)
```


Indica se l'allineamento delle colonne è abilitato per le tabelle Markdown generate. Quando abilitato, le colonne sono allineate aggiungendo spazi al contenuto delle celle con il carattere specificato (tipicamente ' ' per gli spazi). Impostare a '\\0' per disabilitare l'allineamento delle colonne (predefinito).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | char |  |

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

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Indica se calcolare le formule prima di salvare il file markdown.

**Remarks**

Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

### setExportHyperlinkAsReference(boolean value) {#setExportHyperlinkAsReference-boolean-}
```
public void setExportHyperlinkAsReference(boolean value)
```


Indica se esportare i collegamenti ipertestuali usando definizioni di riferimento invece del formato inline. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


Specifica se le immagini vengono salvate in formato Base64 nel Markdown. Il valore predefinito è true.

**Remarks**

Quando questa proprietà è impostata su true, i dati dell'immagine vengono esportati direttamente negli elementi img e non vengono creati file separati.

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

### setLightCellsDataProvider(LightCellsDataProvider value) {#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-}
```
public void setLightCellsDataProvider(LightCellsDataProvider value)
```


Il provider di dati per fornire i dati delle celle durante il salvataggio della cartella di lavoro in modalità leggera.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider) |  |

### setLineSeparator(String value) {#setLineSeparator-java.lang.String-}
```
public void setLineSeparator(String value)
```


Imposta il separatore di riga.

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

### setOfficeMathOutputType(int value) {#setOfficeMathOutputType-int-}
```
public void setOfficeMathOutputType(int value)
```


Indica come gli oggetti OfficeMath vengono esportati in Markdown, il valore predefinito è Immagine.

Vedi [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

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

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Imposta i fogli da renderizzare. Il valore predefinito è tutti i fogli visibili nella cartella di lavoro: [SheetSet.getActive()](../../com.aspose.cells/sheetset\#getActive--).

**Remarks**

Il set è ignorato quando viene utilizzato in [SheetRender](../../com.aspose.cells/sheetrender)

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

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

### setSplitTablesByBlankRow(boolean value) {#setSplitTablesByBlankRow-boolean-}
```
public void setSplitTablesByBlankRow(boolean value)
```


Indica se le righe vuote nel foglio di lavoro devono essere trattate come separatori di tabella durante l'esportazione in Markdown. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Imposta l'IStreamProvider per l'esportazione degli oggetti. Se `null`, gli oggetti esportati saranno salvati nella stessa directory del file di output.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setTableHeaderType(int value) {#setTableHeaderType-int-}
```
public void setTableHeaderType(int value)
```


Imposta come impostare l'intestazione della tabella.

Vedi [MarkdownTableHeaderType](../../com.aspose.cells/markdowntableheadertype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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

