---
title: "GridJsOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta tutte le opzioni di caricamento per GridJs"
type: docs
url: /it/java/com.aspose.gridjs/gridjsoptions/
---

**Inheritance:**
java.lang.Object
```
public class GridJsOptions
```

Rappresenta tutte le opzioni di caricamento per GridJs
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [GridJsOptions()](#GridJsOptions--) |  |
## Campi

| Campo | Descrizione |
| --- | --- |
| [CacheImp](#CacheImp) | Implementazione personalizzata per l'archiviazione della cache, se vuoi memorizzare la cache in modalità streaming, devi impostarla e implementarla. |
| [RedactionUseClientGenerateId](#RedactionUseClientGenerateId) | Indica se utilizzare l'ID generato dal client invece dell'ID reale della forma nelle operazioni correlate alla redazione |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitColumnsOnLoad()](#getAutoFitColumnsOnLoad--) | Indica se adattare automaticamente la larghezza delle colonne durante il caricamento del file, il valore predefinito è false. |
| [getAutoFitRowsHeightOnLoad()](#getAutoFitRowsHeightOnLoad--) | Indica se adattare automaticamente l'altezza delle righe durante il caricamento del file, il valore predefinito è false. |
| [getAutoOptimizeForLargeCells()](#getAutoOptimizeForLargeCells--) | Restituisce se ottimizzare automaticamente le prestazioni di caricamento per i fogli di lavoro con celle grandi. |
| [getBaseRouteName()](#getBaseRouteName--) | Restituisce il nome base dell'URL di percorso per il controller GridJs. Il valore predefinito è GridJs2 |
| [getClass()](#getClass--) |  |
| [getEmptySheetMaxCol()](#getEmptySheetMaxCol--) | Restituisce la colonna massima predefinita per un foglio di lavoro vuoto. |
| [getEmptySheetMaxRow()](#getEmptySheetMaxRow--) | Restituisce la riga massima predefinita per un foglio di lavoro vuoto. |
| [getEnableChartClientRendering()](#getEnableChartClientRendering--) | Restituisce se abilitare il rendering dei grafici lato client. |
| [getFileCacheDirectory()](#getFileCacheDirectory--) | Restituisce la directory della cache per l'archiviazione del file di foglio di calcolo. |
| [getFontFolders()](#getFontFolders--) | Restituisce le cartelle dei font per i font nelle immagini/forme renderizzate. |
| [getIgnoreEmptyContent()](#getIgnoreEmptyContent--) | Restituisce se mostrare l'intervallo massimo che include dati, stile, celle unite e forme. |
| [getIslimitShapeOrImage()](#getIslimitShapeOrImage--) | Restituisce se limitare il conteggio totale di forme/immagini visualizzate in un foglio di lavoro; se impostato su true, GridJs limiterà il conteggio totale di forme o immagini visualizzate in un foglio di lavoro a MaxShapeOrImageCount. Il valore predefinito è true. |
| [getJsonCache()](#getJsonCache--) | Restituisce le opzioni di configurazione della cache JSON. |
| [getLazyLoading()](#getLazyLoading--) | Restituisce se caricare solo il foglio di lavoro attivo, il valore predefinito è false. |
| [getMaxPdfSaveSeconds()](#getMaxPdfSaveSeconds--) | Restituisce il numero massimo di secondi di timeout durante il salvataggio in PDF. |
| [getMaxShapeOrImageCount()](#getMaxShapeOrImageCount--) | Restituisce il conteggio totale di forme o immagini visualizzate nel foglio attivo; ha effetto quando IslimitShapeOrImage=true. |
| [getMaxShapeOrImageWidthOrHeight()](#getMaxShapeOrImageWidthOrHeight--) | Restituisce la larghezza o altezza massima per una forma o un'immagine; GridJs ignorerà la forma o l'immagine con larghezza o altezza superiore a questo valore. Ha effetto quando IslimitShapeOrImage=true. |
| [getMaxTotalShapeOrImageCount()](#getMaxTotalShapeOrImageCount--) | Restituisce il conteggio totale di forme o immagini visualizzate nella cartella di lavoro; ha effetto quando IslimitShapeOrImage=true. |
| [getMessageTopic()](#getMessageTopic--) | Restituisce le destinazioni websocket con prefisso "/topic". Il valore predefinito è "/topic/opr". Utilizzato solo in modalità collaborativa. |
| [getPictureCacheDirectory()](#getPictureCacheDirectory--) | Restituisce la directory della cache per le immagini. |
| [getSameImageDetecting()](#getSameImageDetecting--) | Restituisce se verificare se le immagini hanno la stessa origine, il valore predefinito è true. |
| [getSaveHtmlAsZip()](#getSaveHtmlAsZip--) | Restituisce se salvare il file HTML come archivio zip, il valore predefinito è false. |
| [getShowChartSheet()](#getShowChartSheet--) | Restituisce se mostrare il foglio di lavoro del grafico. |
| [getSkipInvisibleShapes()](#getSkipInvisibleShapes--) | Restituisce se saltare le forme invisibili all'interfaccia utente, il valore predefinito è true. |
| [getUsePrintArea()](#getUsePrintArea--) | Restituisce se utilizzare PageSetup.PrintArea per l'intervallo di visualizzazione dell'interfaccia utente quando il foglio di lavoro ha l'impostazione PageSetup per PrintArea. |
| [hashCode()](#hashCode--) |  |
| [isCollaborative()](#isCollaborative--) | Restituisce se supportare la modifica collaborativa, il valore predefinito è false. |
| [isWasm()](#isWasm--) | Restituisce se GridJs viene eseguito all'interno di un host WebAssembly del browser invece di un processo server. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFitColumnsOnLoad(boolean value)](#setAutoFitColumnsOnLoad-boolean-) | Indica se adattare automaticamente la larghezza delle colonne durante il caricamento del file, il valore predefinito è false. |
| [setAutoFitRowsHeightOnLoad(boolean value)](#setAutoFitRowsHeightOnLoad-boolean-) | Indica se adattare automaticamente l'altezza delle righe durante il caricamento del file, il valore predefinito è false. |
| [setAutoOptimizeForLargeCells(boolean value)](#setAutoOptimizeForLargeCells-boolean-) | Imposta se ottimizzare automaticamente le prestazioni di caricamento per i fogli di lavoro con celle grandi. |
| [setBaseRouteName(String value)](#setBaseRouteName-java.lang.String-) | Imposta il nome base dell'URL di route per il controller GridJs. Il valore predefinito è GridJs2. |
| [setCollaborative(boolean value)](#setCollaborative-boolean-) | Imposta se supportare la modifica collaborativa, il valore predefinito è false. |
| [setEmptySheetMaxCol(int value)](#setEmptySheetMaxCol-int-) | Imposta il numero massimo di colonne predefinito per un foglio di lavoro vuoto. |
| [setEmptySheetMaxRow(int value)](#setEmptySheetMaxRow-int-) | Imposta il numero massimo di righe predefinito per un foglio di lavoro vuoto. |
| [setEnableChartClientRendering(boolean value)](#setEnableChartClientRendering-boolean-) | Imposta se abilitare il rendering dei grafici lato client. |
| [setFileCacheDirectory(String value)](#setFileCacheDirectory-java.lang.String-) | Imposta la directory della cache per la memorizzazione dei file di foglio di calcolo. |
| [setFontFolders(String[] value)](#setFontFolders-java.lang.String---) | Imposta le cartelle dei font per i caratteri nelle immagini/forme renderizzate. |
| [setIgnoreEmptyContent(boolean value)](#setIgnoreEmptyContent-boolean-) | Imposta se mostrare l'intervallo massimo che include dati, stile, celle unite e forme. |
| [setIslimitShapeOrImage(boolean value)](#setIslimitShapeOrImage-boolean-) | Imposta se limitare il conteggio totale di forme/immagini visualizzate in un foglio di lavoro; se impostato su true, GridJs limiterà il conteggio totale di forme o immagini visualizzate in un foglio di lavoro a MaxShapeOrImageCount. Il valore predefinito è true. |
| [setJsonCache(JsonCacheOptions value)](#setJsonCache-com.aspose.gridjs.JsonCacheOptions-) | Imposta le opzioni di configurazione della cache JSON. |
| [setLazyLoading(boolean value)](#setLazyLoading-boolean-) | Imposta se caricare solo il foglio di lavoro attivo, il valore predefinito è false. |
| [setMaxPdfSaveSeconds(int value)](#setMaxPdfSaveSeconds-int-) | Imposta il numero massimo di secondi di timeout quando si salva in PDF. |
| [setMaxShapeOrImageCount(int value)](#setMaxShapeOrImageCount-int-) | Imposta il conteggio totale di forme o immagini visualizzate nel foglio attivo; ha effetto quando IslimitShapeOrImage=true. |
| [setMaxShapeOrImageWidthOrHeight(int value)](#setMaxShapeOrImageWidthOrHeight-int-) | Imposta la larghezza o altezza massima per una forma o un'immagine; GridJs ignorerà le forme o le immagini con larghezza o altezza superiore a questo valore. Ha effetto quando IslimitShapeOrImage=true. |
| [setMaxTotalShapeOrImageCount(int value)](#setMaxTotalShapeOrImageCount-int-) | Imposta il conteggio totale di forme o immagini visualizzate nella cartella di lavoro; ha effetto quando IslimitShapeOrImage=true. |
| [setMessageTopic(String value)](#setMessageTopic-java.lang.String-) | Imposta le destinazioni websocket con prefisso "/topic". Il valore predefinito è "/topic/opr". Utilizzato solo in modalità collaborativa. |
| [setPictureCacheDirectory(String value)](#setPictureCacheDirectory-java.lang.String-) | Imposta la directory della cache per le immagini. |
| [setSameImageDetecting(boolean value)](#setSameImageDetecting-boolean-) | Imposta se verificare se le immagini hanno la stessa origine, il valore predefinito è true. |
| [setSaveHtmlAsZip(boolean value)](#setSaveHtmlAsZip-boolean-) | Imposta se salvare il file HTML come archivio zip, il valore predefinito è false. |
| [setShowChartSheet(boolean value)](#setShowChartSheet-boolean-) | Imposta se mostrare il foglio di lavoro del grafico. |
| [setSkipInvisibleShapes(boolean value)](#setSkipInvisibleShapes-boolean-) | Imposta se saltare le forme invisibili nell'interfaccia utente, il valore predefinito è true. |
| [setUsePrintArea(boolean value)](#setUsePrintArea-boolean-) | Imposta se utilizzare PageSetup.PrintArea per l'intervallo di visualizzazione UI quando il foglio di lavoro ha l'impostazione PageSetup per PrintArea. |
| [setWasm(boolean value)](#setWasm-boolean-) | Imposta se GridJs viene eseguito all'interno di un host WebAssembly del browser invece di un processo server. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsOptions() {#GridJsOptions--}
```
public GridJsOptions()
```


### CacheImp {#CacheImp}
```
public GridCacheForStream CacheImp
```


Implementazione personalizzata per l'archiviazione della cache. Se desideri memorizzare la cache in modalità stream, devi impostarla e implementarla. Un host WebAssembly (IsWasm = true) deve impostarla, perché non esiste un disco locale per la cache di file predefinita.

### RedactionUseClientGenerateId {#RedactionUseClientGenerateId}
```
public boolean RedactionUseClientGenerateId
```


Indica se utilizzare l'ID generato dal client invece dell'ID reale della forma nelle operazioni correlate alla redazione

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
### getAutoFitColumnsOnLoad() {#getAutoFitColumnsOnLoad--}
```
public boolean getAutoFitColumnsOnLoad()
```


Indica se adattare automaticamente la larghezza delle colonne durante il caricamento del file, il valore predefinito è false.

**Returns:**
boolean
### getAutoFitRowsHeightOnLoad() {#getAutoFitRowsHeightOnLoad--}
```
public boolean getAutoFitRowsHeightOnLoad()
```


Indica se adattare automaticamente l'altezza delle righe durante il caricamento del file, il valore predefinito è false.

**Returns:**
boolean
### getAutoOptimizeForLargeCells() {#getAutoOptimizeForLargeCells--}
```
public boolean getAutoOptimizeForLargeCells()
```


Restituisce se ottimizzare automaticamente le prestazioni di caricamento per fogli di lavoro con celle grandi. Ignorerà alcuni stili / bordi per ridurre il tempo di caricamento. Il valore predefinito è true.

**Returns:**
boolean
### getBaseRouteName() {#getBaseRouteName--}
```
public String getBaseRouteName()
```


Restituisce il nome base dell'URL di percorso per il controller GridJs. Il valore predefinito è GridJs2

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEmptySheetMaxCol() {#getEmptySheetMaxCol--}
```
public int getEmptySheetMaxCol()
```


Restituisce il numero massimo di colonne predefinito per un foglio di lavoro vuoto. Il valore predefinito è 15.

**Returns:**
int
### getEmptySheetMaxRow() {#getEmptySheetMaxRow--}
```
public int getEmptySheetMaxRow()
```


Restituisce il numero massimo di righe predefinito per un foglio di lavoro vuoto. Il valore predefinito è 12.

**Returns:**
int
### getEnableChartClientRendering() {#getEnableChartClientRendering--}
```
public boolean getEnableChartClientRendering()
```


Restituisce se abilitare il rendering dei grafici lato client. Se impostato su false, GridJs emetterà solo immagini/forme dei grafici e non richiederà il rendering lato client. Il valore predefinito è true.

**Returns:**
boolean
### getFileCacheDirectory() {#getFileCacheDirectory--}
```
public String getFileCacheDirectory()
```


Restituisce la directory della cache per la memorizzazione del file di foglio di calcolo. È necessario impostarla su un percorso specifico prima di utilizzare GridJs.

**Returns:**
java.lang.String
### getFontFolders() {#getFontFolders--}
```
public String[] getFontFolders()
```


Restituisce le cartelle dei font per i font nelle immagini/forme renderizzate.

**Returns:**
java.lang.String[]
### getIgnoreEmptyContent() {#getIgnoreEmptyContent--}
```
public boolean getIgnoreEmptyContent()
```


Restituisce se mostrare l'intervallo massimo che include dati, stile, celle unite e forme. Se l'ultima riga o colonna contiene celle senza valore e formula ma con stile personalizzato, non mostreremo questa riga/colonna quando questo valore è true\\u9286?\\* il valore predefinito è true.

**Returns:**
boolean
### getIslimitShapeOrImage() {#getIslimitShapeOrImage--}
```
public boolean getIslimitShapeOrImage()
```


Restituisce se limitare il conteggio totale di forme/immagini visualizzate in un foglio di lavoro; se impostato su true, GridJs limiterà il conteggio totale di forme o immagini visualizzate in un foglio di lavoro a MaxShapeOrImageCount. Il valore predefinito è true.

**Returns:**
boolean
### getJsonCache() {#getJsonCache--}
```
public JsonCacheOptions getJsonCache()
```


Restituisce le opzioni di configurazione della cache JSON. Controlla sia la cache in memoria (L1) sia quella su disco (L2) per il JSON del workbook generato.

**Returns:**
[JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions)
### getLazyLoading() {#getLazyLoading--}
```
public boolean getLazyLoading()
```


Restituisce se caricare solo il foglio di lavoro attivo, il valore predefinito è false.

**Returns:**
boolean
### getMaxPdfSaveSeconds() {#getMaxPdfSaveSeconds--}
```
public int getMaxPdfSaveSeconds()
```


Restituisce il numero massimo di secondi di timeout quando si salva in PDF. Il valore predefinito è 10.

**Returns:**
int
### getMaxShapeOrImageCount() {#getMaxShapeOrImageCount--}
```
public int getMaxShapeOrImageCount()
```


Restituisce il conteggio totale delle forme o immagini visualizzate nel foglio attivo, ha effetto quando IslimitShapeOrImage=true. Il valore predefinito è 100.

**Returns:**
int
### getMaxShapeOrImageWidthOrHeight() {#getMaxShapeOrImageWidthOrHeight--}
```
public int getMaxShapeOrImageWidthOrHeight()
```


Restituisce la larghezza o altezza massima per una forma o un'immagine, GridJs ignorerà la forma o l'immagine con larghezza o altezza superiore a questo valore, ha effetto quando IslimitShapeOrImage=true. Il valore predefinito è 10000.

**Returns:**
int
### getMaxTotalShapeOrImageCount() {#getMaxTotalShapeOrImageCount--}
```
public int getMaxTotalShapeOrImageCount()
```


Restituisce il conteggio totale delle forme o immagini visualizzate nel workbook, ha effetto quando IslimitShapeOrImage=true. Il valore predefinito è 300.

**Returns:**
int
### getMessageTopic() {#getMessageTopic--}
```
public String getMessageTopic()
```


Restituisce le destinazioni websocket con prefisso "/topic". Il valore predefinito è "/topic/opr". Utilizzato solo in modalità collaborativa.

**Returns:**
java.lang.String
### getPictureCacheDirectory() {#getPictureCacheDirectory--}
```
public String getPictureCacheDirectory()
```


Restituisce la directory della cache per le immagini. (ha effetto quando GridJsWorkbook.CacheImp è null) il percorso predefinito sarà "\\_piccache" all'interno di FileCacheDirectory.

**Returns:**
java.lang.String
### getSameImageDetecting() {#getSameImageDetecting--}
```
public boolean getSameImageDetecting()
```


Restituisce se verificare se le immagini hanno la stessa origine, il valore predefinito è true.

**Returns:**
boolean
### getSaveHtmlAsZip() {#getSaveHtmlAsZip--}
```
public boolean getSaveHtmlAsZip()
```


Restituisce se salvare il file HTML come archivio zip, il valore predefinito è false.

**Returns:**
boolean
### getShowChartSheet() {#getShowChartSheet--}
```
public boolean getShowChartSheet()
```


Restituisce se mostrare il foglio di lavoro dei grafici. Il valore predefinito è false.

**Returns:**
boolean
### getSkipInvisibleShapes() {#getSkipInvisibleShapes--}
```
public boolean getSkipInvisibleShapes()
```


Restituisce se saltare le forme invisibili all'interfaccia utente, il valore predefinito è true.

**Returns:**
boolean
### getUsePrintArea() {#getUsePrintArea--}
```
public boolean getUsePrintArea()
```


Restituisce se utilizzare PageSetup.PrintArea per l'intervallo di visualizzazione UI quando il foglio di lavoro ha l'impostazione PageSetup per PrintArea. Il valore predefinito è false.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCollaborative() {#isCollaborative--}
```
public boolean isCollaborative()
```


Restituisce se supportare la modifica collaborativa, il valore predefinito è false.

**Returns:**
boolean
### isWasm() {#isWasm--}
```
public boolean isWasm()
```


Restituisce se GridJs viene eseguito all'interno di un host WebAssembly del browser invece di un processo server. Quando true, non vengono utilizzati FileCacheDirectory / disco / percorso di thread di interruzione, e la cache dei file deve provenire da CacheImp, perché un host browser non ha disco locale. Seleziona i percorsi di codice a runtime, così un Aspose.Cells.GridJs.dll serve entrambi gli host. Il valore predefinito è false.

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




### setAutoFitColumnsOnLoad(boolean value) {#setAutoFitColumnsOnLoad-boolean-}
```
public void setAutoFitColumnsOnLoad(boolean value)
```


Indica se adattare automaticamente la larghezza delle colonne durante il caricamento del file, il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutoFitRowsHeightOnLoad(boolean value) {#setAutoFitRowsHeightOnLoad-boolean-}
```
public void setAutoFitRowsHeightOnLoad(boolean value)
```


Indica se adattare automaticamente l'altezza delle righe durante il caricamento del file, il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutoOptimizeForLargeCells(boolean value) {#setAutoOptimizeForLargeCells-boolean-}
```
public void setAutoOptimizeForLargeCells(boolean value)
```


Imposta se ottimizzare automaticamente le prestazioni di caricamento per fogli di lavoro con celle grandi. Ignorerà alcuni stili / bordi per ridurre il tempo di caricamento. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setBaseRouteName(String value) {#setBaseRouteName-java.lang.String-}
```
public void setBaseRouteName(String value)
```


Imposta il nome base dell'URL di route per il controller GridJs. Il valore predefinito è GridJs2.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCollaborative(boolean value) {#setCollaborative-boolean-}
```
public void setCollaborative(boolean value)
```


Imposta se supportare la modifica collaborativa, il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEmptySheetMaxCol(int value) {#setEmptySheetMaxCol-int-}
```
public void setEmptySheetMaxCol(int value)
```


Imposta il numero massimo di colonne predefinito per un foglio di lavoro vuoto. Il valore predefinito è 15.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setEmptySheetMaxRow(int value) {#setEmptySheetMaxRow-int-}
```
public void setEmptySheetMaxRow(int value)
```


Imposta il numero massimo di righe predefinito per un foglio di lavoro vuoto. Il valore predefinito è 12.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setEnableChartClientRendering(boolean value) {#setEnableChartClientRendering-boolean-}
```
public void setEnableChartClientRendering(boolean value)
```


Imposta se abilitare il rendering dei grafici lato client. Se impostato su false, GridJs emetterà solo immagini/forme dei grafici e non richiederà il rendering lato client. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFileCacheDirectory(String value) {#setFileCacheDirectory-java.lang.String-}
```
public void setFileCacheDirectory(String value)
```


Imposta la directory della cache per la memorizzazione del file di foglio di calcolo. È necessario impostarla su un percorso specifico prima di utilizzare GridJs.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setFontFolders(String[] value) {#setFontFolders-java.lang.String---}
```
public void setFontFolders(String[] value)
```


Imposta le cartelle dei font per i caratteri nelle immagini/forme renderizzate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String[] |  |

### setIgnoreEmptyContent(boolean value) {#setIgnoreEmptyContent-boolean-}
```
public void setIgnoreEmptyContent(boolean value)
```


Imposta se mostrare l'intervallo massimo che include dati, stile, celle unite e forme. Se l'ultima riga o colonna contiene celle senza valore e formula ma con stile personalizzato, non mostreremo questa riga/colonna quando questo valore è true\\u9286?\\* il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setIslimitShapeOrImage(boolean value) {#setIslimitShapeOrImage-boolean-}
```
public void setIslimitShapeOrImage(boolean value)
```


Imposta se limitare il conteggio totale di forme/immagini visualizzate in un foglio di lavoro; se impostato su true, GridJs limiterà il conteggio totale di forme o immagini visualizzate in un foglio di lavoro a MaxShapeOrImageCount. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setJsonCache(JsonCacheOptions value) {#setJsonCache-com.aspose.gridjs.JsonCacheOptions-}
```
public void setJsonCache(JsonCacheOptions value)
```


Imposta le opzioni di configurazione della cache JSON. Controlla sia il comportamento della cache in memoria (L1) che su disco (L2) per il JSON del workbook generato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions) |  |

### setLazyLoading(boolean value) {#setLazyLoading-boolean-}
```
public void setLazyLoading(boolean value)
```


Imposta se caricare solo il foglio di lavoro attivo, il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setMaxPdfSaveSeconds(int value) {#setMaxPdfSaveSeconds-int-}
```
public void setMaxPdfSaveSeconds(int value)
```


Imposta i secondi massimi di timeout durante il salvataggio in PDF. Il valore predefinito è 10.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMaxShapeOrImageCount(int value) {#setMaxShapeOrImageCount-int-}
```
public void setMaxShapeOrImageCount(int value)
```


Imposta il conteggio totale delle forme o immagini visualizzate nel foglio attivo, ha effetto quando IslimitShapeOrImage=true. Il valore predefinito è 100.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMaxShapeOrImageWidthOrHeight(int value) {#setMaxShapeOrImageWidthOrHeight-int-}
```
public void setMaxShapeOrImageWidthOrHeight(int value)
```


Imposta la larghezza o altezza massima per una forma o un'immagine, GridJs ignorerà le forme o le immagini con larghezza o altezza superiore a questo valore, ha effetto quando IslimitShapeOrImage=true. Il valore predefinito è 10000.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMaxTotalShapeOrImageCount(int value) {#setMaxTotalShapeOrImageCount-int-}
```
public void setMaxTotalShapeOrImageCount(int value)
```


Imposta il conteggio totale delle forme o immagini visualizzate nel workbook, ha effetto quando IslimitShapeOrImage=true. Il valore predefinito è 300.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMessageTopic(String value) {#setMessageTopic-java.lang.String-}
```
public void setMessageTopic(String value)
```


Imposta le destinazioni websocket con prefisso "/topic". Il valore predefinito è "/topic/opr". Utilizzato solo in modalità collaborativa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPictureCacheDirectory(String value) {#setPictureCacheDirectory-java.lang.String-}
```
public void setPictureCacheDirectory(String value)
```


Imposta la directory della cache per le immagini. (ha effetto quando GridJsWorkbook.CacheImp è null) il percorso predefinito sarà "\_piccache" all'interno di FileCacheDirectory.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setSameImageDetecting(boolean value) {#setSameImageDetecting-boolean-}
```
public void setSameImageDetecting(boolean value)
```


Imposta se verificare se le immagini hanno la stessa origine, il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSaveHtmlAsZip(boolean value) {#setSaveHtmlAsZip-boolean-}
```
public void setSaveHtmlAsZip(boolean value)
```


Imposta se salvare il file HTML come archivio zip, il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowChartSheet(boolean value) {#setShowChartSheet-boolean-}
```
public void setShowChartSheet(boolean value)
```


Imposta se mostrare il foglio di lavoro del grafico. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSkipInvisibleShapes(boolean value) {#setSkipInvisibleShapes-boolean-}
```
public void setSkipInvisibleShapes(boolean value)
```


Imposta se saltare le forme invisibili nell'interfaccia utente, il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setUsePrintArea(boolean value) {#setUsePrintArea-boolean-}
```
public void setUsePrintArea(boolean value)
```


Imposta se utilizzare PageSetup.PrintArea per l'intervallo di visualizzazione UI quando il foglio di lavoro ha l'impostazione PageSetup per PrintArea. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setWasm(boolean value) {#setWasm-boolean-}
```
public void setWasm(boolean value)
```


Imposta se GridJs viene eseguito all'interno di un host WebAssembly del browser invece di un processo server. Quando true, non viene utilizzato alcun percorso FileCacheDirectory / disco / thread di interruzione, e la cache dei file deve provenire da CacheImp, poiché un host browser non ha disco locale. Seleziona i percorsi di codice a runtime, quindi un unico Aspose.Cells.GridJs.dll serve entrambi gli host. Il valore predefinito è false.

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

