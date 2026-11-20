---
title: "OoxmlSaveOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni di salvataggio del file Office Open XML."
type: docs
url: /it/java/com.aspose.cells/ooxmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class OoxmlSaveOptions extends SaveOptions
```

Rappresenta le opzioni di salvataggio del file Office Open XML.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [OoxmlSaveOptions()](#OoxmlSaveOptions--) | Crea le opzioni per salvare il file Office Open XML. |
| [OoxmlSaveOptions(int saveFormat)](#OoxmlSaveOptions-int-) | Crea le opzioni per salvare il file Office Open XML. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAsFlatOpc()](#getAsFlatOpc--) | Indica se salvare come file OPC flat che può essere generato da Open XML SDK. |
| [getCachedFileFolder()](#getCachedFileFolder--) | La cartella per i file temporanei che possono essere usati come cache dei dati. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Rendi il workbook vuoto dopo aver salvato il file. |
| [getCompressionType()](#getCompressionType--) | Ottiene il tipo di compressione per il file ooxml. |
| [getCreateDirectory()](#getCreateDirectory--) | Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [getEmbedOoxmlAsOleObject()](#getEmbedOoxmlAsOleObject--) | Indica se incorporare i file Ooxml di OleObject come oggetto ole. |
| [getEnableZip64()](#getEnableZip64--) | Usa le estensioni ZIP64 durante la scrittura di archivi zip, se necessario. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indica se crittografare le proprietà del documento quando si salva come file .xls. |
| [getExportCellName()](#getExportCellName--) | Indica se esportare il nome della cella in un file Excel2007 .xlsx (.xlsm, .xltx, .xltm). |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | Il provider di dati per salvare la cartella di lavoro in modalità leggera. |
| [getMergeAreas()](#getMergeAreas--) | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indica se memorizzare nella cache i dati più recenti del grafico. |
| [getSaveFormat()](#getSaveFormat--) | Ottiene il formato di salvataggio del file. |
| [getSortExternalNames()](#getSortExternalNames--) | Indica se ordinare i nomi definiti esterni prima di salvare il file. |
| [getSortNames()](#getSortNames--) | Indica se ordinare i nomi definiti prima di salvare il file. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indica se aggiornare le impostazioni di SmartArt. |
| [getUpdateZoom()](#getUpdateZoom--) | Indica se aggiornare il fattore di scala prima di salvare il file se le proprietà PageSetup.FitToPagesWide e PageSetup.FitToPagesTall controllano come il foglio di lavoro viene scalato. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indica se convalidare le celle unite prima di salvare il file. |
| [getWarningCallback()](#getWarningCallback--) | Ottiene il callback di avviso. |
| [getWpsCompatibility()](#getWpsCompatibility--) | Indica se rendere il file xls più compatibile con WPS. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAsFlatOpc(boolean value)](#setAsFlatOpc-boolean-) | Indica se salvare come file OPC flat che può essere generato da Open XML SDK. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | La cartella per i file temporanei che possono essere usati come cache dei dati. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [setClearData(boolean value)](#setClearData-boolean-) | Rendi il workbook vuoto dopo aver salvato il file. |
| [setCompressionType(int value)](#setCompressionType-int-) | Imposta il tipo di compressione per il file ooxml. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [setEmbedOoxmlAsOleObject(boolean value)](#setEmbedOoxmlAsOleObject-boolean-) | Indica se incorporare i file Ooxml di OleObject come oggetto ole. |
| [setEnableZip64(boolean value)](#setEnableZip64-boolean-) | Usa le estensioni ZIP64 durante la scrittura di archivi zip, se necessario. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indica se crittografare le proprietà del documento quando si salva come file .xls. |
| [setExportCellName(boolean value)](#setExportCellName-boolean-) | Indica se esportare il nome della cella in un file Excel2007 .xlsx (.xlsm, .xltx, .xltm). |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | Il provider di dati per salvare la cartella di lavoro in modalità leggera. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indica se memorizzare nella cache i dati più recenti del grafico. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indica se ordinare i nomi definiti esterni prima di salvare il file. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indica se ordinare i nomi definiti prima di salvare il file. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indica se aggiornare le impostazioni di SmartArt. |
| [setUpdateZoom(boolean value)](#setUpdateZoom-boolean-) | Indica se aggiornare il fattore di scala prima di salvare il file se le proprietà PageSetup.FitToPagesWide e PageSetup.FitToPagesTall controllano come il foglio di lavoro viene scalato. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indica se convalidare le celle unite prima di salvare il file. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Imposta la callback di avviso. |
| [setWpsCompatibility(boolean value)](#setWpsCompatibility-boolean-) | Indica se rendere il file xls più compatibile con WPS. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### OoxmlSaveOptions() {#OoxmlSaveOptions--}
```
public OoxmlSaveOptions()
```


Crea le opzioni per salvare il file Office Open XML.

### OoxmlSaveOptions(int saveFormat) {#OoxmlSaveOptions-int-}
```
public OoxmlSaveOptions(int saveFormat)
```


Crea le opzioni per salvare il file Office Open XML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Il formato del file. Deve essere uno dei seguenti tipi: [SaveFormat.XLSX](../../com.aspose.cells/saveformat\#XLSX), [SaveFormat.XLTX](../../com.aspose.cells/saveformat\#XLTX), [SaveFormat.XLAM](../../com.aspose.cells/saveformat\#XLAM), [SaveFormat.XLSM](../../com.aspose.cells/saveformat\#XLSM) o [SaveFormat.XLTM](../../com.aspose.cells/saveformat\#XLTM), altrimenti il formato salvato verrà impostato automaticamente su [SaveFormat.XLSX](../../com.aspose.cells/saveformat\#XLSX). |

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
### getAsFlatOpc() {#getAsFlatOpc--}
```
public boolean getAsFlatOpc()
```


Indica se salvare come file OPC flat che può essere generato da Open XML SDK.

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
### getCompressionType() {#getCompressionType--}
```
public int getCompressionType()
```


Ottiene il tipo di compressione per il file ooxml.

Vedi [OoxmlCompressionType](../../com.aspose.cells/ooxmlcompressiontype).

**Remarks**

Il valore predefinito è OoxmlCompressionType.Level2.

**Returns:**
int
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file.

**Remarks**

Il valore predefinito è false.

**Returns:**
boolean
### getEmbedOoxmlAsOleObject() {#getEmbedOoxmlAsOleObject--}
```
public boolean getEmbedOoxmlAsOleObject()
```


Indica se incorporare i file Ooxml di OleObject come oggetto ole.

**Remarks**

Solo per OleObject.

**Returns:**
boolean
### getEnableZip64() {#getEnableZip64--}
```
public boolean getEnableZip64()
```


Usa le estensioni ZIP64 durante la scrittura di archivi zip, se necessario.

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
### getExportCellName() {#getExportCellName--}
```
public boolean getExportCellName()
```


Indica se esportare il nome della cella in un file Excel2007 .xlsx (.xlsm, .xltx, .xltm). Se il file di output può essere accessibile da SQL Server DTS, questo valore deve essere true. Impostare il valore su false aumenterà notevolmente le prestazioni e ridurrà le dimensioni del file quando si creano file di grandi dimensioni. Il valore predefinito è true.

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
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Indica se aggiornare l'impostazione Smart Art. Il valore predefinito è false.

**Remarks**

Ha effetto solo dopo aver chiamato il metodo Shape.GetResultOfSmartArt() e quando le forme memorizzate nella cache esistono nel file modello.

**Returns:**
boolean
### getUpdateZoom() {#getUpdateZoom--}
```
public boolean getUpdateZoom()
```


Indica se aggiornare il fattore di scala prima di salvare il file se le proprietà PageSetup.FitToPagesWide e PageSetup.FitToPagesTall controllano come il foglio di lavoro viene scalato.

**Remarks**

Il valore predefinito è false per le prestazioni.

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
### getWpsCompatibility() {#getWpsCompatibility--}
```
public boolean getWpsCompatibility()
```


Indica se rendere il file xls più compatibile con WPS.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà WorkbookSetting.WpsCompatibility. Questo metodo verrà rimosso tra 12 mesi a partire da dicembre 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

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




### setAsFlatOpc(boolean value) {#setAsFlatOpc-boolean-}
```
public void setAsFlatOpc(boolean value)
```


Indica se salvare come file OPC flat che può essere generato da Open XML SDK.

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

### setCompressionType(int value) {#setCompressionType-int-}
```
public void setCompressionType(int value)
```


Imposta il tipo di compressione per il file ooxml.

Vedi [OoxmlCompressionType](../../com.aspose.cells/ooxmlcompressiontype).

**Remarks**

Il valore predefinito è OoxmlCompressionType.Level2.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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

### setEmbedOoxmlAsOleObject(boolean value) {#setEmbedOoxmlAsOleObject-boolean-}
```
public void setEmbedOoxmlAsOleObject(boolean value)
```


Indica se incorporare i file Ooxml di OleObject come oggetto ole.

**Remarks**

Solo per OleObject.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableZip64(boolean value) {#setEnableZip64-boolean-}
```
public void setEnableZip64(boolean value)
```


Usa le estensioni ZIP64 durante la scrittura di archivi zip, se necessario.

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

### setExportCellName(boolean value) {#setExportCellName-boolean-}
```
public void setExportCellName(boolean value)
```


Indica se esportare il nome della cella in un file Excel2007 .xlsx (.xlsm, .xltx, .xltm). Se il file di output può essere accessibile da SQL Server DTS, questo valore deve essere true. Impostare il valore su false aumenterà notevolmente le prestazioni e ridurrà le dimensioni del file quando si creano file di grandi dimensioni. Il valore predefinito è true.

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

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Indica se memorizzare nella cache i dati più recenti del grafico.

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

### setUpdateZoom(boolean value) {#setUpdateZoom-boolean-}
```
public void setUpdateZoom(boolean value)
```


Indica se aggiornare il fattore di scala prima di salvare il file se le proprietà PageSetup.FitToPagesWide e PageSetup.FitToPagesTall controllano come il foglio di lavoro viene scalato.

**Remarks**

Il valore predefinito è false per le prestazioni.

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

### setWpsCompatibility(boolean value) {#setWpsCompatibility-boolean-}
```
public void setWpsCompatibility(boolean value)
```


Indica se rendere il file xls più compatibile con WPS.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà WorkbookSetting.WpsCompatibility. Questo metodo verrà rimosso tra 12 mesi a partire da dicembre 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

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

