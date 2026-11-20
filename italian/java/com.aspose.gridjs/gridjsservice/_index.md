---
title: "GridJsService"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Fornisce le API di operazione di base utilizzate nelle azioni del controller."
type: docs
url: /it/java/com.aspose.gridjs/gridjsservice/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.gridjs.IGridJsService](../../com.aspose.gridjs/igridjsservice)
```
public class GridJsService implements IGridJsService
```

Fornisce le API di operazione di base utilizzate nelle azioni del controller.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [GridJsService(GridJsOptions options)](#GridJsService-com.aspose.gridjs.GridJsOptions-) | Il costruttore predefinito per GridJsService |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addImage(String p, String uid, InputStream filestream)](#addImage-java.lang.String-java.lang.String-java.io.InputStream-) | Applica l'operazione di aggiunta immagine da file locale. |
| [addImageByURL(String p, String uid, InputStream filestream, String imageurl)](#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Applica l'operazione di aggiunta immagine da file locale. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Verifica se l'istanza della cartella di lavoro è nella cache di memoria. Questo metodo è applicabile solo in modalità Collaborativa. |
| [clearAllJsonCache()](#clearAllJsonCache--) | Cancella tutte le voci della cache JSON (memoria e disco). |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | Cancella tutte le voci della cache JSON appartenenti all'ID univoco specificato. |
| [copyImage(String p, String uid)](#copyImage-java.lang.String-java.lang.String-) | Applica l'operazione di copia immagine. |
| [destroy()](#destroy--) | Questo metodo è solo per Java, implementa il metodo destroy in DisposableBean, che verrà chiamato automaticamente da Spring al termine della richiesta; in realtà chiamerà il metodo Dispose. |
| [detailFileJsonWithUid(String filePath, String uid)](#detailFileJsonWithUid-java.lang.String-java.lang.String-) | Ottiene la stringa JSON per il file tramite l'ID univoco specificato. |
| [detailStreamJson(OutputStream stream, String filePath)](#detailStreamJson-java.io.OutputStream-java.lang.String-) | Scrive la stringa JSON del file nello stream. |
| [detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)](#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Scrive la stringa JSON del file nello stream tramite l'ID univoco specificato. |
| [dispose()](#dispose--) | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino di risorse non gestite. |
| [download(String p, String uid, String filename)](#download-java.lang.String-java.lang.String-java.lang.String-) | Applica l'operazione di download del file |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFile(String fileid)](#getFile-java.lang.String-) | Ottieni lo stream del file |
| [getSettings()](#getSettings--) | Rappresenta le impostazioni della cartella di lavoro. |
| [hashCode()](#hashCode--) |  |
| [image(String uid, String picid)](#image-java.lang.String-java.lang.String-) | Ottieni lo stream dell'immagine. |
| [imageUrl(String baseURL, String picid, String uid)](#imageUrl-java.lang.String-java.lang.String-java.lang.String-) | Ottiene l'URL dell'immagine. |
| [lazyLoadingJson(String sheetName, String uid)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Ottiene la stringa JSON del foglio specificato nel file dalla cache usando l'ID univoco specificato. |
| [lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)](#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-) | Scrive la stringa JSON del foglio specificato nel file dalla cache usando l'ID univoco specificato nello stream.. |
| [load(String uid, String filename)](#load-java.lang.String-java.lang.String-) | Ottiene la stringa JSON del file dalla cache usando l'ID univoco specificato, imposta il nome file di output nel JSON. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [ole(String uid, String sheetname, int oleid, String label)](#ole-java.lang.String-java.lang.String-int-java.lang.String-) | Ottiene i dati dell'array di byte dell'oggetto OLE incorporato. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridjs.GridWorkbookSettings-) | Rappresenta le impostazioni della cartella di lavoro. |
| [toString()](#toString--) |  |
| [translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)](#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-) | Traduci tutti i valori stringa nella lingua di destinazione nel foglio di lavoro |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Applica l'operazione di aggiornamento. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsService(GridJsOptions options) {#GridJsService-com.aspose.gridjs.GridJsOptions-}
```
public GridJsService(GridJsOptions options)
```


Il costruttore predefinito per GridJsService

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | [GridJsOptions](../../com.aspose.gridjs/gridjsoptions) |  |

### addImage(String p, String uid, InputStream filestream) {#addImage-java.lang.String-java.lang.String-java.io.InputStream-}
```
public String addImage(String p, String uid, InputStream filestream)
```


Applica l'operazione di aggiunta immagine da file locale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| p | java.lang.String | Il parametro stringa JSON |
| uid | java.lang.String | L'id univoco per la cache del file. |
| filestream | java.io.InputStream | Il flusso file dell'immagine |

**Returns:**
java.lang.String - Il risultato della stringa JSON
### addImageByURL(String p, String uid, InputStream filestream, String imageurl) {#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-}
```
public String addImageByURL(String p, String uid, InputStream filestream, String imageurl)
```


Applica l'operazione di aggiunta immagine da file locale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| p | java.lang.String | Il parametro stringa JSON |
| uid | java.lang.String | L'id univoco per la cache del file. |
| filestream | java.io.InputStream | Il flusso file dell'immagine |
| imageurl | java.lang.String | Specifica l'URL dell'immagine. |

**Returns:**
java.lang.String - Il risultato della stringa JSON
### checkInCacheForCollaborative(String uid) {#checkInCacheForCollaborative-java.lang.String-}
```
public boolean checkInCacheForCollaborative(String uid)
```


Verifica se l'istanza della cartella di lavoro è nella cache di memoria. Questo metodo è applicabile solo in modalità Collaborativa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String |  |

**Returns:**
boolean -
### clearAllJsonCache() {#clearAllJsonCache--}
```
public void clearAllJsonCache()
```


Cancella tutte le voci della cache JSON (memoria e disco).

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public void clearJsonCacheForUid(String uid)
```


Cancella tutte le voci della cache JSON appartenenti all'ID univoco specificato. Chiama questo metodo dopo aver modificato il file sorgente al di fuori del flusso normale, così la prossima richiesta rigenera il JSON.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'id univoco per la cache del file. |

### copyImage(String p, String uid) {#copyImage-java.lang.String-java.lang.String-}
```
public String copyImage(String p, String uid)
```


Applica l'operazione di copia immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| p | java.lang.String | Il parametro stringa JSON |
| uid | java.lang.String | L'id univoco per la cache del file. |

**Returns:**
java.lang.String - Il risultato della stringa JSON
### destroy() {#destroy--}
```
public void destroy()
```


Questo metodo è solo per Java, implementa il metodo destroy in DisposableBean, che verrà chiamato automaticamente da Spring al termine della richiesta; in realtà chiamerà il metodo Dispose.

### detailFileJsonWithUid(String filePath, String uid) {#detailFileJsonWithUid-java.lang.String-java.lang.String-}
```
public StringBuilder detailFileJsonWithUid(String filePath, String uid)
```


Ottiene la stringa JSON per il file tramite l'ID univoco specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | Il percorso completo del file |
| uid | java.lang.String | L'id univoco per la cache del file. |

**Returns:**
java.lang.StringBuilder
### detailStreamJson(OutputStream stream, String filePath) {#detailStreamJson-java.io.OutputStream-java.lang.String-}
```
public void detailStreamJson(OutputStream stream, String filePath)
```


Scrive la stringa JSON del file nello stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso che verrà scritto |
| filePath | java.lang.String | Il percorso completo del file |

### detailStreamJsonWithUid(OutputStream stream, String filePath, String uid) {#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)
```


Scrive la stringa JSON del file nello stream tramite l'ID univoco specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso che verrà scritto |
| filePath | java.lang.String | Il percorso completo del file |
| uid | java.lang.String | L'id univoco per la cache del file. |

### dispose() {#dispose--}
```
public void dispose()
```


Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino di risorse non gestite.

### download(String p, String uid, String filename) {#download-java.lang.String-java.lang.String-java.lang.String-}
```
public String download(String p, String uid, String filename)
```


Applica l'operazione di download del file

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| p | java.lang.String | Il parametro JSON |
| uid | java.lang.String | L'id univoco per la cache del file. |
| nome file | java.lang.String | Il nome del file |

**Returns:**
java.lang.String - L'URL del file
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFile(String fileid) {#getFile-java.lang.String-}
```
public InputStream getFile(String fileid)
```


Ottieni lo stream del file

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileid | java.lang.String | l'ID del file |

**Returns:**
java.io.InputStream - Il flusso del file
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Rappresenta le impostazioni della cartella di lavoro.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### image(String uid, String picid) {#image-java.lang.String-java.lang.String-}
```
public InputStream image(String uid, String picid)
```


Ottieni lo stream dell'immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'id univoco per la cache del file. |
| picid | java.lang.String | L'ID dell'immagine. |

**Returns:**
java.io.InputStream - Il flusso dell'immagine
### imageUrl(String baseURL, String picid, String uid) {#imageUrl-java.lang.String-java.lang.String-java.lang.String-}
```
public String imageUrl(String baseURL, String picid, String uid)
```


Ottiene l'URL dell'immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| baseURL | java.lang.String | L'URL di base dell'azione. |
| picid | java.lang.String | L'ID dell'immagine. |
| uid | java.lang.String | L'id univoco per la cache del file. |

**Returns:**
java.lang.String - L'URL dell'immagine
### lazyLoadingJson(String sheetName, String uid) {#lazyLoadingJson-java.lang.String-java.lang.String-}
```
public StringBuilder lazyLoadingJson(String sheetName, String uid)
```


Ottiene la stringa JSON del foglio specificato nel file dalla cache usando l'ID univoco specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetName | java.lang.String | il nome del foglio. |
| uid | java.lang.String | L'id univoco per la cache del file. |

**Returns:**
java.lang.StringBuilder
### lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid) {#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)
```


Scrive la stringa JSON del foglio specificato nel file dalla cache usando l'ID univoco specificato nello stream..

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso che verrà scritto |
| sheetName | java.lang.String | Il nome del foglio. |
| uid | java.lang.String | L'id univoco per la cache del file. |

### load(String uid, String filename) {#load-java.lang.String-java.lang.String-}
```
public String load(String uid, String filename)
```


Ottiene la stringa JSON del file dalla cache usando l'ID univoco specificato, imposta il nome file di output nel JSON.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'id univoco per la cache del file. |
| nome file | java.lang.String | Specifica il nome del file nel JSON. Se impostato a null, il nome file predefinito è: book1. |

**Returns:**
java.lang.String - La stringa JSON
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### ole(String uid, String sheetname, int oleid, String label) {#ole-java.lang.String-java.lang.String-int-java.lang.String-}
```
public byte[] ole(String uid, String sheetname, int oleid, String label)
```


Ottiene i dati dell'array di byte dell'oggetto OLE incorporato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'id univoco per la cache del file. |
| sheetname | java.lang.String | Il nome del foglio di lavoro. |
| oleid | int | L'ID per l'oggetto OLE incorporato. |
| label | java.lang.String | L'etichetta visualizzata dell'oggetto OLE incorporato. |

**Returns:**
byte[] - I dati dell'array di byte dell'oggetto OLE incorporato.
### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridjs.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Rappresenta le impostazioni della cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage) {#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-}
```
public String translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)
```


Traduci tutti i valori stringa nella lingua di destinazione nel foglio di lavoro

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'id univoco per la cache del file. |
| sheetName | java.lang.String | Il nome del foglio |
| translator | [ITextTranslator](../../com.aspose.gridjs/itexttranslator) | Il traduttore che implementa la funzione di traduzione |
| targetLanguage | java.lang.String | La lingua di destinazione |

**Returns:**
java.lang.String -
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public String updateCell(String p, String uid)
```


Applica l'operazione di aggiornamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| p | java.lang.String | La stringa di formato JSON dell'operazione di aggiornamento. |
| uid | java.lang.String | L'id univoco per la cache del file. |

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

