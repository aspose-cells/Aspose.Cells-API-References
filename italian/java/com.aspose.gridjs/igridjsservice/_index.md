---
title: "IGridJsService"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta l'interfaccia delle API di operazione di base utilizzata nelle azioni del controller."
type: docs
url: /it/java/com.aspose.gridjs/igridjsservice/
---
```
public interface IGridJsService
```

Rappresenta l'interfaccia delle API di operazione di base utilizzata nelle azioni del controller.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addImage(String p, String uid, InputStream filestream)](#addImage-java.lang.String-java.lang.String-java.io.InputStream-) | Applica l'operazione di aggiunta immagine da file locale. |
| [addImageByURL(String p, String uid, InputStream filestream, String imageurl)](#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Applica l'operazione di aggiunta immagine da URL remoto. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Verifica se l'istanza della cartella di lavoro è nella cache di memoria. Questo metodo è applicabile solo in modalità Collaborativa. |
| [clearAllJsonCache()](#clearAllJsonCache--) | Cancella tutte le voci della cache JSON (memoria e disco). |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | Cancella tutte le voci della cache JSON appartenenti all'ID univoco specificato. |
| [copyImage(String p, String uid)](#copyImage-java.lang.String-java.lang.String-) | Applica l'operazione di copia immagine. |
| [detailFileJsonWithUid(String filePath, String uid)](#detailFileJsonWithUid-java.lang.String-java.lang.String-) | Ottiene la stringa JSON per il file tramite l'ID univoco specificato. |
| [detailStreamJson(OutputStream stream, String filePath)](#detailStreamJson-java.io.OutputStream-java.lang.String-) | Scrivi la stringa JSON per la cartella di lavoro nello stream |
| [detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)](#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Scrive la stringa JSON del file nello stream tramite l'ID univoco specificato. |
| [dispose()](#dispose--) |  |
| [download(String p, String uid, String filename)](#download-java.lang.String-java.lang.String-java.lang.String-) | Applica l'operazione di download del file |
| [getFile(String fileid)](#getFile-java.lang.String-) | Ottieni lo stream del file |
| [image(String uid, String picid)](#image-java.lang.String-java.lang.String-) | Ottieni lo stream dell'immagine. |
| [imageUrl(String baseURL, String picid, String uid)](#imageUrl-java.lang.String-java.lang.String-java.lang.String-) | Ottiene l'URL dell'immagine. |
| [lazyLoadingJson(String sheetName, String uid)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Ottiene la stringa JSON del foglio specificato nel file dalla cache usando l'ID univoco specificato. |
| [lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)](#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-) | Scrive la stringa JSON del foglio specificato nel file dalla cache usando l'ID univoco specificato nello stream.. |
| [load(String uid, String filename)](#load-java.lang.String-java.lang.String-) | Ottiene la stringa JSON del file dalla cache usando l'ID univoco specificato, imposta il nome file di output nel JSON. |
| [ole(String uid, String sheetname, int oleid, String label)](#ole-java.lang.String-java.lang.String-int-java.lang.String-) | Ottiene i dati dell'array di byte dell'oggetto OLE incorporato. |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Applica l'operazione di aggiornamento. |
### addImage(String p, String uid, InputStream filestream) {#addImage-java.lang.String-java.lang.String-java.io.InputStream-}
```
public abstract String addImage(String p, String uid, InputStream filestream)
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
public abstract String addImageByURL(String p, String uid, InputStream filestream, String imageurl)
```


Applica l'operazione di aggiunta immagine da URL remoto.

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
public abstract boolean checkInCacheForCollaborative(String uid)
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
public abstract void clearAllJsonCache()
```


Cancella tutte le voci della cache JSON (memoria e disco).

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public abstract void clearJsonCacheForUid(String uid)
```


Cancella tutte le voci della cache JSON appartenenti all'ID univoco specificato. Chiama questo metodo dopo aver modificato il file sorgente al di fuori del flusso normale, così la prossima richiesta rigenera il JSON.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'id univoco per la cache del file. |

### copyImage(String p, String uid) {#copyImage-java.lang.String-java.lang.String-}
```
public abstract String copyImage(String p, String uid)
```


Applica l'operazione di copia immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| p | java.lang.String | Il parametro stringa JSON |
| uid | java.lang.String | L'id univoco per la cache del file. |

**Returns:**
java.lang.String - Il risultato della stringa JSON
### detailFileJsonWithUid(String filePath, String uid) {#detailFileJsonWithUid-java.lang.String-java.lang.String-}
```
public abstract StringBuilder detailFileJsonWithUid(String filePath, String uid)
```


Ottiene la stringa JSON per il file tramite l'ID univoco specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | Il percorso del file |
| uid | java.lang.String | L'id univoco per la cache del file. |

**Returns:**
java.lang.StringBuilder
### detailStreamJson(OutputStream stream, String filePath) {#detailStreamJson-java.io.OutputStream-java.lang.String-}
```
public abstract void detailStreamJson(OutputStream stream, String filePath)
```


Scrivi la stringa JSON per la cartella di lavoro nello stream

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso che verrà scritto |
| filePath | java.lang.String | Il percorso del file |

### detailStreamJsonWithUid(OutputStream stream, String filePath, String uid) {#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public abstract void detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)
```


Scrive la stringa JSON del file nello stream tramite l'ID univoco specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso che verrà scritto |
| filePath | java.lang.String | Il percorso del file |
| uid | java.lang.String | L'id univoco per la cache del file. |

### dispose() {#dispose--}
```
public abstract void dispose()
```




### download(String p, String uid, String filename) {#download-java.lang.String-java.lang.String-java.lang.String-}
```
public abstract String download(String p, String uid, String filename)
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
### getFile(String fileid) {#getFile-java.lang.String-}
```
public abstract InputStream getFile(String fileid)
```


Ottieni lo stream del file

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileid | java.lang.String | l'ID del file |

**Returns:**
java.io.InputStream - Il flusso del file
### image(String uid, String picid) {#image-java.lang.String-java.lang.String-}
```
public abstract InputStream image(String uid, String picid)
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
public abstract String imageUrl(String baseURL, String picid, String uid)
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
public abstract StringBuilder lazyLoadingJson(String sheetName, String uid)
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
public abstract void lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)
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
public abstract String load(String uid, String filename)
```


Ottiene la stringa JSON del file dalla cache usando l'ID univoco specificato, imposta il nome file di output nel JSON.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'id univoco per la cache del file. |
| nome file | java.lang.String | Specifica il nome del file nel JSON. Se impostato a null, il nome file predefinito è: book1. |

**Returns:**
java.lang.String - La stringa JSON
### ole(String uid, String sheetname, int oleid, String label) {#ole-java.lang.String-java.lang.String-int-java.lang.String-}
```
public abstract byte[] ole(String uid, String sheetname, int oleid, String label)
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
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public abstract String updateCell(String p, String uid)
```


Applica l'operazione di aggiornamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| p | java.lang.String | La stringa di formato JSON dell'operazione di aggiornamento. |
| uid | java.lang.String | L'id univoco per la cache del file. |

**Returns:**
java.lang.String
