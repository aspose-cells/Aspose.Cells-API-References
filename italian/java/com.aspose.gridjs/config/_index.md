---
title: "Config"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta tutte le impostazioni statiche per GridJs"
type: docs
url: /it/java/com.aspose.gridjs/config/
---

**Inheritance:**
java.lang.Object
```
public class Config
```

Rappresenta tutte le impostazioni statiche per GridJs
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Config()](#Config--) |  |
## Campi

| Campo | Descrizione |
| --- | --- |
| [RedactionUseClientGenerateId](#RedactionUseClientGenerateId) | Indica se utilizzare l'ID generato dal client invece dell'ID reale della forma nelle operazioni correlate alla redazione |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitColumnsOnLoad()](#getAutoFitColumnsOnLoad--) | Indica se adattare automaticamente la larghezza delle colonne durante il caricamento del file. |
| [getAutoFitRowsHeightOnLoad()](#getAutoFitRowsHeightOnLoad--) | Indica se adattare automaticamente le altezze delle righe durante il caricamento del file. |
| [getAutoOptimizeForLargeCells()](#getAutoOptimizeForLargeCells--) | Restituisce se ottimizzare automaticamente le prestazioni di caricamento per i fogli di lavoro con celle grandi. |
| [getBaseRouteName()](#getBaseRouteName--) | Ottiene il nome del percorso base per l'URL del controller GridJs. il valore predefinito è "/GridJs2". |
| [getClass()](#getClass--) |  |
| [getEmptySheetMaxCol()](#getEmptySheetMaxCol--) | Restituisce la colonna massima predefinita per un foglio di lavoro vuoto. |
| [getEmptySheetMaxRow()](#getEmptySheetMaxRow--) | Restituisce la riga massima predefinita per un foglio di lavoro vuoto. |
| [getEnableChartClientRendering()](#getEnableChartClientRendering--) | Restituisce se abilitare il rendering dei grafici lato client. |
| [getFileCacheDirectory()](#getFileCacheDirectory--) | Restituisce la directory della cache per l'archiviazione del file di foglio di calcolo. |
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
| [setAutoFitColumnsOnLoad(boolean value)](#setAutoFitColumnsOnLoad-boolean-) | Indica se adattare automaticamente la larghezza delle colonne durante il caricamento del file. |
| [setAutoFitRowsHeightOnLoad(boolean value)](#setAutoFitRowsHeightOnLoad-boolean-) | Indica se adattare automaticamente le altezze delle righe durante il caricamento del file. |
| [setAutoOptimizeForLargeCells(boolean value)](#setAutoOptimizeForLargeCells-boolean-) | Imposta se ottimizzare automaticamente le prestazioni di caricamento per i fogli di lavoro con celle grandi. |
| [setBaseRouteName(String value)](#setBaseRouteName-java.lang.String-) | Imposta il nome del percorso base per l'URL del controller GridJs. il valore predefinito è "/GridJs2". |
| [setCollaborative(boolean value)](#setCollaborative-boolean-) | Imposta se supportare la modifica collaborativa, il valore predefinito è false. |
| [setEmptySheetMaxCol(int value)](#setEmptySheetMaxCol-int-) | Imposta il numero massimo di colonne predefinito per un foglio di lavoro vuoto. |
| [setEmptySheetMaxRow(int value)](#setEmptySheetMaxRow-int-) | Imposta il numero massimo di righe predefinito per un foglio di lavoro vuoto. |
| [setEnableChartClientRendering(boolean value)](#setEnableChartClientRendering-boolean-) | Imposta se abilitare il rendering dei grafici lato client. |
| [setFileCacheDirectory(String value)](#setFileCacheDirectory-java.lang.String-) | Imposta la directory della cache per la memorizzazione dei file di foglio di calcolo. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Imposta la cartella delle font |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Imposta le cartelle dei font |
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
### Config() {#Config--}
```
public Config()
```


### RedactionUseClientGenerateId {#RedactionUseClientGenerateId}
```
public static boolean RedactionUseClientGenerateId
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
public static boolean getAutoFitColumnsOnLoad()
```


Indica se adattare automaticamente le larghezze delle colonne durante il caricamento del file. Il valore predefinito è `false`. Avviso: impostare questo su `true` eseguirà un'operazione di adattamento automatico di tutte le colonne dopo il caricamento, il che può avere un impatto notevole sulle prestazioni.

**Returns:**
boolean
### getAutoFitRowsHeightOnLoad() {#getAutoFitRowsHeightOnLoad--}
```
public static boolean getAutoFitRowsHeightOnLoad()
```


Indica se adattare automaticamente le altezze delle righe durante il caricamento del file. Il valore predefinito è `false`. Avviso: impostare questo su `true` eseguirà un'operazione di adattamento automatico di tutte le righe dopo il caricamento, il che può avere un impatto notevole sulle prestazioni.

**Returns:**
boolean
### getAutoOptimizeForLargeCells() {#getAutoOptimizeForLargeCells--}
```
public static boolean getAutoOptimizeForLargeCells()
```


Restituisce se ottimizzare automaticamente le prestazioni di caricamento per fogli di lavoro con celle grandi. Ignorerà alcuni stili / bordi per ridurre il tempo di caricamento. Il valore predefinito è true.

**Returns:**
boolean
### getBaseRouteName() {#getBaseRouteName--}
```
public static String getBaseRouteName()
```


Ottiene il nome del percorso base per l'URL del controller GridJs. il valore predefinito è "/GridJs2".

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
public static int getEmptySheetMaxCol()
```


Restituisce il numero massimo di colonne predefinito per un foglio di lavoro vuoto. Il valore predefinito è 15.

**Returns:**
int
### getEmptySheetMaxRow() {#getEmptySheetMaxRow--}
```
public static int getEmptySheetMaxRow()
```


Restituisce il numero massimo di righe predefinito per un foglio di lavoro vuoto. Il valore predefinito è 12.

**Returns:**
int
### getEnableChartClientRendering() {#getEnableChartClientRendering--}
```
public static boolean getEnableChartClientRendering()
```


Ottiene se abilitare il rendering dei grafici lato client. Se impostato su false, GridJs tornerà a utilizzare solo immagini/forme di grafico generate dal server. il valore predefinito è true.

**Returns:**
boolean
### getFileCacheDirectory() {#getFileCacheDirectory--}
```
public static String getFileCacheDirectory()
```


Restituisce la directory della cache per la memorizzazione del file di foglio di calcolo. È necessario impostarla su un percorso specifico prima di utilizzare GridJs.

**Returns:**
java.lang.String
### getIgnoreEmptyContent() {#getIgnoreEmptyContent--}
```
public static boolean getIgnoreEmptyContent()
```


Restituisce se mostrare l'intervallo massimo che include dati, stile, celle unite e forme. Se l'ultima riga o colonna contiene celle senza valore e formula ma con stile personalizzato, non mostreremo questa riga/colonna quando questo valore è true\\u9286?\\* il valore predefinito è true.

**Returns:**
boolean
### getIslimitShapeOrImage() {#getIslimitShapeOrImage--}
```
public static boolean getIslimitShapeOrImage()
```


Restituisce se limitare il conteggio totale di forme/immagini visualizzate in un foglio di lavoro; se impostato su true, GridJs limiterà il conteggio totale di forme o immagini visualizzate in un foglio di lavoro a MaxShapeOrImageCount. Il valore predefinito è true.

**Returns:**
boolean
### getJsonCache() {#getJsonCache--}
```
public static JsonCacheOptions getJsonCache()
```


Restituisce le opzioni di configurazione della cache JSON. Controlla sia la cache in memoria (L1) sia quella su disco (L2) per il JSON del workbook generato.

**Returns:**
[JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions)
### getLazyLoading() {#getLazyLoading--}
```
public static boolean getLazyLoading()
```


Restituisce se caricare solo il foglio di lavoro attivo, il valore predefinito è false.

**Returns:**
boolean
### getMaxPdfSaveSeconds() {#getMaxPdfSaveSeconds--}
```
public static int getMaxPdfSaveSeconds()
```


Restituisce il numero massimo di secondi di timeout quando si salva in PDF. Il valore predefinito è 10.

**Returns:**
int
### getMaxShapeOrImageCount() {#getMaxShapeOrImageCount--}
```
public static int getMaxShapeOrImageCount()
```


Restituisce il conteggio totale delle forme o immagini visualizzate nel foglio attivo, ha effetto quando IslimitShapeOrImage=true. Il valore predefinito è 100.

**Returns:**
int
### getMaxShapeOrImageWidthOrHeight() {#getMaxShapeOrImageWidthOrHeight--}
```
public static int getMaxShapeOrImageWidthOrHeight()
```


Restituisce la larghezza o altezza massima per una forma o un'immagine, GridJs ignorerà la forma o l'immagine con larghezza o altezza superiore a questo valore, ha effetto quando IslimitShapeOrImage=true. Il valore predefinito è 10000.

**Returns:**
int
### getMaxTotalShapeOrImageCount() {#getMaxTotalShapeOrImageCount--}
```
public static int getMaxTotalShapeOrImageCount()
```


Restituisce il conteggio totale delle forme o immagini visualizzate nel workbook, ha effetto quando IslimitShapeOrImage=true. Il valore predefinito è 300.

**Returns:**
int
### getMessageTopic() {#getMessageTopic--}
```
public static String getMessageTopic()
```


Restituisce le destinazioni websocket con prefisso "/topic". Il valore predefinito è "/topic/opr". Utilizzato solo in modalità collaborativa.

**Returns:**
java.lang.String
### getPictureCacheDirectory() {#getPictureCacheDirectory--}
```
public static String getPictureCacheDirectory()
```


Restituisce la directory della cache per le immagini. (ha effetto quando GridJsWorkbook.CacheImp è null) il percorso predefinito sarà "\\_piccache" all'interno di FileCacheDirectory.

**Returns:**
java.lang.String
### getSameImageDetecting() {#getSameImageDetecting--}
```
public static boolean getSameImageDetecting()
```


Restituisce se verificare se le immagini hanno la stessa origine, il valore predefinito è true.

**Returns:**
boolean
### getSaveHtmlAsZip() {#getSaveHtmlAsZip--}
```
public static boolean getSaveHtmlAsZip()
```


Restituisce se salvare il file HTML come archivio zip, il valore predefinito è false.

**Returns:**
boolean
### getShowChartSheet() {#getShowChartSheet--}
```
public static boolean getShowChartSheet()
```


Restituisce se mostrare il foglio di lavoro dei grafici. Il valore predefinito è false.

**Returns:**
boolean
### getSkipInvisibleShapes() {#getSkipInvisibleShapes--}
```
public static boolean getSkipInvisibleShapes()
```


Restituisce se saltare le forme invisibili all'interfaccia utente, il valore predefinito è true.

**Returns:**
boolean
### getUsePrintArea() {#getUsePrintArea--}
```
public static boolean getUsePrintArea()
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
public static boolean isCollaborative()
```


Restituisce se supportare la modifica collaborativa, il valore predefinito è false.

**Returns:**
boolean
### isWasm() {#isWasm--}
```
public static boolean isWasm()
```


Ottiene se GridJs viene eseguito all'interno di un host WebAssembly del browser invece di un processo server. Quando è true, non viene utilizzato alcun percorso FileCacheDirectory / disco / thread di interruzione e la cache dei file deve provenire da GridJsOptions.CacheImp. GridJsOptions.IsWasm imposta questo quando il servizio GridJs viene costruito, quindi un unico Aspose.Cells.GridJs.dll serve entrambi gli host. il valore predefinito è false.

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
public static void setAutoFitColumnsOnLoad(boolean value)
```


Indica se adattare automaticamente le larghezze delle colonne durante il caricamento del file. Il valore predefinito è `false`. Avviso: impostare questo su `true` eseguirà un'operazione di adattamento automatico di tutte le colonne dopo il caricamento, il che può avere un impatto notevole sulle prestazioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutoFitRowsHeightOnLoad(boolean value) {#setAutoFitRowsHeightOnLoad-boolean-}
```
public static void setAutoFitRowsHeightOnLoad(boolean value)
```


Indica se adattare automaticamente le altezze delle righe durante il caricamento del file. Il valore predefinito è `false`. Avviso: impostare questo su `true` eseguirà un'operazione di adattamento automatico di tutte le righe dopo il caricamento, il che può avere un impatto notevole sulle prestazioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutoOptimizeForLargeCells(boolean value) {#setAutoOptimizeForLargeCells-boolean-}
```
public static void setAutoOptimizeForLargeCells(boolean value)
```


Imposta se ottimizzare automaticamente le prestazioni di caricamento per fogli di lavoro con celle grandi. Ignorerà alcuni stili / bordi per ridurre il tempo di caricamento. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setBaseRouteName(String value) {#setBaseRouteName-java.lang.String-}
```
public static void setBaseRouteName(String value)
```


Imposta il nome del percorso base per l'URL del controller GridJs. il valore predefinito è "/GridJs2".

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCollaborative(boolean value) {#setCollaborative-boolean-}
```
public static void setCollaborative(boolean value)
```


Imposta se supportare la modifica collaborativa, il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEmptySheetMaxCol(int value) {#setEmptySheetMaxCol-int-}
```
public static void setEmptySheetMaxCol(int value)
```


Imposta il numero massimo di colonne predefinito per un foglio di lavoro vuoto. Il valore predefinito è 15.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setEmptySheetMaxRow(int value) {#setEmptySheetMaxRow-int-}
```
public static void setEmptySheetMaxRow(int value)
```


Imposta il numero massimo di righe predefinito per un foglio di lavoro vuoto. Il valore predefinito è 12.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setEnableChartClientRendering(boolean value) {#setEnableChartClientRendering-boolean-}
```
public static void setEnableChartClientRendering(boolean value)
```


Imposta se abilitare il rendering dei grafici lato client. Se impostato su false, GridJs tornerà a utilizzare solo immagini/forme di grafico generate dal server. il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFileCacheDirectory(String value) {#setFileCacheDirectory-java.lang.String-}
```
public static void setFileCacheDirectory(String value)
```


Imposta la directory della cache per la memorizzazione del file di foglio di calcolo. È necessario impostarla su un percorso specifico prima di utilizzare GridJs.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```


Imposta la cartella delle font

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontFolder | java.lang.String | La cartella che contiene i font TrueType. |
| recursive | boolean | Determina se eseguire o meno la scansione delle sottocartelle. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


Imposta le cartelle dei font

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Le cartelle che contengono i font TrueType. |
| recursive | boolean | Determina se eseguire o meno la scansione delle sottocartelle. |

### setIgnoreEmptyContent(boolean value) {#setIgnoreEmptyContent-boolean-}
```
public static void setIgnoreEmptyContent(boolean value)
```


Imposta se mostrare l'intervallo massimo che include dati, stile, celle unite e forme. Se l'ultima riga o colonna contiene celle senza valore e formula ma con stile personalizzato, non mostreremo questa riga/colonna quando questo valore è true\\u9286?\\* il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setIslimitShapeOrImage(boolean value) {#setIslimitShapeOrImage-boolean-}
```
public static void setIslimitShapeOrImage(boolean value)
```


Imposta se limitare il conteggio totale di forme/immagini visualizzate in un foglio di lavoro; se impostato su true, GridJs limiterà il conteggio totale di forme o immagini visualizzate in un foglio di lavoro a MaxShapeOrImageCount. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setJsonCache(JsonCacheOptions value) {#setJsonCache-com.aspose.gridjs.JsonCacheOptions-}
```
public static void setJsonCache(JsonCacheOptions value)
```


Imposta le opzioni di configurazione della cache JSON. Controlla sia il comportamento della cache in memoria (L1) che su disco (L2) per il JSON del workbook generato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions) |  |

### setLazyLoading(boolean value) {#setLazyLoading-boolean-}
```
public static void setLazyLoading(boolean value)
```


Imposta se caricare solo il foglio di lavoro attivo, il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setMaxPdfSaveSeconds(int value) {#setMaxPdfSaveSeconds-int-}
```
public static void setMaxPdfSaveSeconds(int value)
```


Imposta i secondi massimi di timeout durante il salvataggio in PDF. Il valore predefinito è 10.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMaxShapeOrImageCount(int value) {#setMaxShapeOrImageCount-int-}
```
public static void setMaxShapeOrImageCount(int value)
```


Imposta il conteggio totale delle forme o immagini visualizzate nel foglio attivo, ha effetto quando IslimitShapeOrImage=true. Il valore predefinito è 100.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMaxShapeOrImageWidthOrHeight(int value) {#setMaxShapeOrImageWidthOrHeight-int-}
```
public static void setMaxShapeOrImageWidthOrHeight(int value)
```


Imposta la larghezza o altezza massima per una forma o un'immagine, GridJs ignorerà le forme o le immagini con larghezza o altezza superiore a questo valore, ha effetto quando IslimitShapeOrImage=true. Il valore predefinito è 10000.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMaxTotalShapeOrImageCount(int value) {#setMaxTotalShapeOrImageCount-int-}
```
public static void setMaxTotalShapeOrImageCount(int value)
```


Imposta il conteggio totale delle forme o immagini visualizzate nel workbook, ha effetto quando IslimitShapeOrImage=true. Il valore predefinito è 300.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMessageTopic(String value) {#setMessageTopic-java.lang.String-}
```
public static void setMessageTopic(String value)
```


Imposta le destinazioni websocket con prefisso "/topic". Il valore predefinito è "/topic/opr". Utilizzato solo in modalità collaborativa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPictureCacheDirectory(String value) {#setPictureCacheDirectory-java.lang.String-}
```
public static void setPictureCacheDirectory(String value)
```


Imposta la directory della cache per le immagini. (ha effetto quando GridJsWorkbook.CacheImp è null) il percorso predefinito sarà "\_piccache" all'interno di FileCacheDirectory.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setSameImageDetecting(boolean value) {#setSameImageDetecting-boolean-}
```
public static void setSameImageDetecting(boolean value)
```


Imposta se verificare se le immagini hanno la stessa origine, il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSaveHtmlAsZip(boolean value) {#setSaveHtmlAsZip-boolean-}
```
public static void setSaveHtmlAsZip(boolean value)
```


Imposta se salvare il file HTML come archivio zip, il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowChartSheet(boolean value) {#setShowChartSheet-boolean-}
```
public static void setShowChartSheet(boolean value)
```


Imposta se mostrare il foglio di lavoro del grafico. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSkipInvisibleShapes(boolean value) {#setSkipInvisibleShapes-boolean-}
```
public static void setSkipInvisibleShapes(boolean value)
```


Imposta se saltare le forme invisibili nell'interfaccia utente, il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setUsePrintArea(boolean value) {#setUsePrintArea-boolean-}
```
public static void setUsePrintArea(boolean value)
```


Imposta se utilizzare PageSetup.PrintArea per l'intervallo di visualizzazione UI quando il foglio di lavoro ha l'impostazione PageSetup per PrintArea. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setWasm(boolean value) {#setWasm-boolean-}
```
public static void setWasm(boolean value)
```


Imposta se GridJs viene eseguito all'interno di un host WebAssembly del browser invece di un processo server. Quando è true, non viene utilizzato alcun percorso FileCacheDirectory / disco / thread di interruzione e la cache dei file deve provenire da GridJsOptions.CacheImp. GridJsOptions.IsWasm imposta questo quando il servizio GridJs viene costruito, quindi un unico Aspose.Cells.GridJs.dll serve entrambi gli host. il valore predefinito è false.

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

