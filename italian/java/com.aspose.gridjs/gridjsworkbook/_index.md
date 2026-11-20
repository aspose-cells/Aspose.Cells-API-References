---
title: "GridJsWorkbook"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta la classe principale di ingresso per GridJs"
type: docs
url: /it/java/com.aspose.gridjs/gridjsworkbook/
---

**Inheritance:**
java.lang.Object
```
public class GridJsWorkbook
```

Rappresenta la classe principale di ingresso per GridJs
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [GridJsWorkbook()](#GridJsWorkbook--) | Crea una nuova istanza di GridJsWorkbook. |
## Campi

| Campo | Descrizione |
| --- | --- |
| [CacheImp](#CacheImp) | Implementazione personalizzata per l'archiviazione della cache, se vuoi memorizzare la cache in modalità streaming, devi impostarla e implementarla. |
| [CalculateEngine](#CalculateEngine) | Implementazione personalizzata per il motore di calcolo, se vuoi eseguire calcoli personalizzati, devi impostarla e implementarla. |
| [PICTURE_TYPE](#PICTURE-TYPE) | valore costante per il tipo dell'immagine |
| [UpdateMonitor](#UpdateMonitor) | Ottiene/Imposta il monitor di aggiornamento per tracciare l'operazione di aggiornamento |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [burnRedactionFile(String excelFilePath, String uid)](#burnRedactionFile-java.lang.String-java.lang.String-) | Applica (applies) tutte le operazioni di redazione nella cartella di lavoro rimuovendo le forme di redazione e le loro forme target o cancellando i contenuti dell'intervallo di celle target. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Verifica se l'istanza della cartella di lavoro è nella cache di memoria. Questo metodo è applicabile solo in modalità Collaborativa. |
| [clearAllJsonCache()](#clearAllJsonCache--) | \\u5a13\\u5474\\u6ace\\u93b5\\u20ac\\u93c8? |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | \\u93cd\\u89c4\\u5d41 uid \\u5a13\\u5474\\u6ace JSON \\u7f02\\u64b3\\u74e8\\u951b\\u5822\\u6564\\u6d5c? |
| [copyImageOrShape(String uid, String p)](#copyImageOrShape-java.lang.String-java.lang.String-) | Copia immagine o forma. |
| [dispose()](#dispose--) | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino di risorse non gestite. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [errorJson(String msg)](#errorJson-java.lang.String-) | Ottiene la stringa del messaggio di errore in formato JSON. |
| [exportToJson()](#exportToJson--) | Ottiene la stringa JSON dai dati in memoria, il nome file predefinito nel JSON è: book1. |
| [exportToJson(String filename)](#exportToJson-java.lang.String-) | Ottiene la stringa JSON dai dati in memoria, imposta il nome file di output nel JSON. |
| [exportToJsonStringBuilder(String filename)](#exportToJsonStringBuilder-java.lang.String-) | Ottiene la stringa JSON dai dati in memoria, imposta il nome file di output nel JSON. |
| [exportToJsonStringBuilder(String filename, String uid)](#exportToJsonStringBuilder-java.lang.String-java.lang.String-) |  |
| [getCacheDirectory()](#getCacheDirectory--) | Restituisce la directory della cache per l'archiviazione del file di foglio di calcolo. |
| [getClass()](#getClass--) |  |
| [getGridLoadFormat(String extension)](#getGridLoadFormat-java.lang.String-) | Ottiene il formato di caricamento dall'estensione del file |
| [getImageStream(String uid, String picid, String cachedir)](#getImageStream-java.lang.String-java.lang.String-java.lang.String-) | Ottieni lo stream dell'immagine. |
| [getImageUrl(String uid, String picid, String delimiter)](#getImageUrl-java.lang.String-java.lang.String-java.lang.String-) | Ottiene l'URL dell'immagine. |
| [getJsonByUid(String uid, String filename)](#getJsonByUid-java.lang.String-java.lang.String-) | Ottiene la stringa JSON del file dalla cache usando l'ID univoco specificato, imposta il nome file di output nel JSON. |
| [getOle(String uid, String sheetname, int oleid, String label)](#getOle-java.lang.String-java.lang.String-int-java.lang.String-) | Ottiene i dati dell'array di byte dell'oggetto OLE incorporato. |
| [getSettings()](#getSettings--) | Rappresenta le impostazioni della cartella di lavoro. |
| [getSheetJsonWithCache(String uid, String sheetName, String fileName)](#getSheetJsonWithCache-java.lang.String-java.lang.String-java.lang.String-) | \\u947e\\u5cf0\\u5f47\\u93b8\\u56e7\\u757e foglio \\u9428? |
| [getUidForFile(String fileName)](#getUidForFile-java.lang.String-) | Genera un nuovo ID univoco per la cache dei file utilizzando il nome file fornito. |
| [getWorkbookJsonWithCache(String uid, String fileName)](#getWorkbookJsonWithCache-java.lang.String-java.lang.String-) | \\u947e\\u5cf0\\u5f47\\u93c1\\u7fe0\\u91dc\\u5bb8\\u30e4\\u7d94\\u7ee8\\u8de8\\u6b91 JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b? |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream filestream, int format)](#importExcelFile-java.io.InputStream-int-) | Importa il file Excel dallo stream del file con il formato di caricamento. |
| [importExcelFile(InputStream filestream, int format, String password)](#importExcelFile-java.io.InputStream-int-java.lang.String-) | Importa il file Excel dallo stream del file con il formato di caricamento e password di apertura. |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | Importa il file Excel dal percorso del file. |
| [importExcelFile(String uid, InputStream filestream, int format)](#importExcelFile-java.lang.String-java.io.InputStream-int-) | Importa il file Excel dallo stream del file. |
| [importExcelFile(String uid, InputStream filestream, int format, String password)](#importExcelFile-java.lang.String-java.io.InputStream-int-java.lang.String-) | Importa il file Excel dallo stream del file con il formato di caricamento e password di apertura. |
| [importExcelFile(String uid, String fileName)](#importExcelFile-java.lang.String-java.lang.String-) | Importa il file Excel dal percorso del file. |
| [importExcelFile(String uid, String fileName, String password)](#importExcelFile-java.lang.String-java.lang.String-java.lang.String-) | Importa il file Excel dal percorso del file e password di apertura. |
| [importExcelFileFromJson(String json)](#importExcelFileFromJson-java.lang.String-) | Importa il file Excel da una stringa in formato JSON. |
| [insertImage(String uid, String p, InputStream s, String imageUrl)](#insertImage-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Inserisce un'immagine nel foglio di lavoro dallo stream del file o dall'URL (deve essere fornito lo stream del file o l'URL) oppure inserisce una forma, quando p.type è uno di AutoShapeType |
| [jsonToStream(OutputStream stream, String filename)](#jsonToStream-java.io.OutputStream-java.lang.String-) | Genera JSON dal Workbook in memoria e lo scrive nello stream specificato. |
| [jsonToStream(OutputStream stream, String filename, String uid)](#jsonToStream-java.io.OutputStream-java.lang.String-java.lang.String-) |  |
| [jsonToStreamByUid(OutputStream stream, String uid, String filename)](#jsonToStreamByUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Recupera la stringa JSON del file dalla cache usando l'ID univoco specificato, imposta il nome file di output nel JSON e lo scrive nello stream. |
| [lazyLoadingJson(String uid, String sheetName)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Ottiene la stringa JSON del foglio specificato nel file dalla cache usando l'ID univoco specificato. |
| [lazyLoadingStream(OutputStream stream, String uid, String sheetName)](#lazyLoadingStream-java.io.OutputStream-java.lang.String-java.lang.String-) | Recupera la stringa JSON del foglio specificato nel file dalla cache usando l'ID univoco specificato e la scrive nello stream. |
| [mergeExcelFileFromJson(String uid, String json)](#mergeExcelFileFromJson-java.lang.String-java.lang.String-) | Applica un aggiornamento batch ai dati in memoria. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr)](#redactFile-java.lang.String-java.lang.String-java.lang.String---) | Esegue la redazione di un file Excel basata su un array di operazioni JSON. |
| [saveToCacheWithFileName(String uid, String filename, String password)](#saveToCacheWithFileName-java.lang.String-java.lang.String-java.lang.String-) | Salva i dati in memoria nel file di cache con il nome file specificato e imposta anche la password di apertura; il formato di salvataggio è basato sull'estensione del nome file. |
| [saveToExcelFile(OutputStream stream)](#saveToExcelFile-java.io.OutputStream-) | Salva i dati in memoria nello sream, basato sul formato originale del file. |
| [saveToExcelFile(String path)](#saveToExcelFile-java.lang.String-) | Salva i dati in memoria nel percorso del file; se il file ha un'estensione, il formato di salvataggio è basato sull'estensione del file. |
| [saveToHtml(OutputStream stream)](#saveToHtml-java.io.OutputStream-) | Salva i dati in memoria nello sream, il formato di salvataggio è html |
| [saveToHtml(String path)](#saveToHtml-java.lang.String-) | Salva i dati in memoria nel percorso del file, il formato di salvataggio è html. |
| [saveToPdf(OutputStream stream)](#saveToPdf-java.io.OutputStream-) | Salva i dati in memoria nello sream, il formato di salvataggio è pdf. |
| [saveToPdf(String path)](#saveToPdf-java.lang.String-) | Salva i dati in memoria nel percorso file, il formato di salvataggio è pdf. |
| [saveToXlsx(OutputStream stream)](#saveToXlsx-java.io.OutputStream-) | Salva i dati in memoria nello stream, il formato di salvataggio è xlsx. |
| [saveToXlsx(String path)](#saveToXlsx-java.lang.String-) | Salva i dati in memoria nel percorso file, il formato di salvataggio è xlsx. |
| [setCacheDirectory(String value)](#setCacheDirectory-java.lang.String-) | Imposta la directory della cache per la memorizzazione dei file di foglio di calcolo. |
| [setImageUrlBase(String baseImageURL)](#setImageUrlBase-java.lang.String-) | Imposta l'URL di azione per ottenere l'immagine di base dal controller. |
| [setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds)](#setInterruptMonitorForLoad-com.aspose.gridjs.GridInterruptMonitor-int-) | Imposta InterruptMonitor per l'operazione di caricamento. |
| [setInterruptMonitorForSave(GridInterruptMonitor monitor)](#setInterruptMonitorForSave-com.aspose.gridjs.GridInterruptMonitor-) | Imposta InterruptMonitor per l'operazione di salvataggio. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridjs.GridWorkbookSettings-) | Rappresenta le impostazioni della cartella di lavoro. |
| [setTransParentView(String excelFilePath, String uid, boolean isTransparent)](#setTransParentView-java.lang.String-java.lang.String-boolean-) | Imposta la trasparenza delle forme di redazione nella cartella di lavoro. |
| [toString()](#toString--) |  |
| [translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)](#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-) | Traduci tutti i valori stringa nella lingua di destinazione nel foglio di lavoro |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Applica l'operazione di aggiornamento. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsWorkbook() {#GridJsWorkbook--}
```
public GridJsWorkbook()
```


Crea una nuova istanza di GridJsWorkbook.

### CacheImp {#CacheImp}
```
public static GridCacheForStream CacheImp
```


Implementazione personalizzata per l'archiviazione della cache, se vuoi memorizzare la cache in modalità streaming, devi impostarla e implementarla.

### CalculateEngine {#CalculateEngine}
```
public static GridAbstractCalculationEngine CalculateEngine
```


Implementazione personalizzata per il motore di calcolo, se vuoi eseguire calcoli personalizzati, devi impostarla e implementarla.

### PICTURE_TYPE {#PICTURE-TYPE}
```
public static final String PICTURE_TYPE
```


valore costante per il tipo dell'immagine

### UpdateMonitor {#UpdateMonitor}
```
public static GridUpdateMonitor UpdateMonitor
```


Ottiene/Imposta il monitor di aggiornamento per tracciare l'operazione di aggiornamento

### burnRedactionFile(String excelFilePath, String uid) {#burnRedactionFile-java.lang.String-java.lang.String-}
```
public void burnRedactionFile(String excelFilePath, String uid)
```


Applica (applies) tutte le operazioni di redazione nella cartella di lavoro rimuovendo le forme di redazione e le loro forme target o cancellando i contenuti dell'intervallo di celle target.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| excelFilePath | java.lang.String | Il percorso del file Excel. |
| uid | java.lang.String | L'identificatore univoco per la cartella di lavoro. Se nullo o vuoto, verrà generato un nuovo uid basato sul percorso del file. |

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


\\u5a13\\u5474\\u6ace\\u93b5\\u20ac\\u93c8?JSON \\u7f02\\u64b3\\u74e8

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public void clearJsonCacheForUid(String uid)
```


\\u93cd\\u89c4\\u5d41 uid \\u5a13\\u5474\\u6ace JSON \\u7f02\\u64b3\\u74e8\\u951b\\u5822\\u6564\\u6d5c?UpdateCell \\u7edb\\u590a\\u5f67\\u93c8?uid \\u9428\\u52eb\\u6e80\\u93c5\\ue224\\u7d1a

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |

### copyImageOrShape(String uid, String p) {#copyImageOrShape-java.lang.String-java.lang.String-}
```
public String copyImageOrShape(String uid, String p)
```


Copia immagine o forma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'id univoco per la cache del file. |
| p | java.lang.String | La stringa JSON per l'operazione che specifica la posizione della cella, contiene il nome del foglio di lavoro, la riga in alto a sinistra, la colonna in alto a sinistra per l'immagine o la forma\\u951b\\u5b94tc \{name:'sheet1',ri:1,ci:1,srcid:2,srcname:'sheet2',isshape:true\} |

**Returns:**
java.lang.String - La stringa JSON della nuova immagine copiata
### dispose() {#dispose--}
```
public void dispose()
```


Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino di risorse non gestite.

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
### errorJson(String msg) {#errorJson-java.lang.String-}
```
public String errorJson(String msg)
```


Ottiene la stringa del messaggio di errore in formato JSON.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| msg | java.lang.String | Il messaggio di errore. |

**Returns:**
java.lang.String - La stringa JSON.
### exportToJson() {#exportToJson--}
```
public String exportToJson()
```


Ottiene la stringa JSON dai dati in memoria, il nome file predefinito nel JSON è: book1.

**Returns:**
java.lang.String - La stringa JSON.
### exportToJson(String filename) {#exportToJson-java.lang.String-}
```
public String exportToJson(String filename)
```


Ottiene la stringa JSON dai dati in memoria, imposta il nome file di output nel JSON.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome file | java.lang.String | Specifica il nome del file nel JSON. Se impostato a null, il nome file predefinito è: book1.. |

**Returns:**
java.lang.String - La stringa JSON.
### exportToJsonStringBuilder(String filename) {#exportToJsonStringBuilder-java.lang.String-}
```
public StringBuilder exportToJsonStringBuilder(String filename)
```


Ottiene la stringa JSON dai dati in memoria, imposta il nome file di output nel JSON.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome file | java.lang.String | Specifica il nome del file nel JSON. Se impostato a null, il nome file predefinito è: book1.. |

**Returns:**
java.lang.StringBuilder - Il JSON StringBuilder.
### exportToJsonStringBuilder(String filename, String uid) {#exportToJsonStringBuilder-java.lang.String-java.lang.String-}
```
public StringBuilder exportToJsonStringBuilder(String filename, String uid)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome file | java.lang.String |  |
| uid | java.lang.String |  |

**Returns:**
java.lang.StringBuilder
### getCacheDirectory() {#getCacheDirectory--}
```
public String getCacheDirectory()
```


Ottiene la directory cache per la memorizzazione del file di foglio di calcolo. se non è impostata, utilizzeremo la proprietà statica da [Config.getFileCacheDirectory()](../../com.aspose.gridjs/config\#getFileCacheDirectory--) o [CacheImp](../../com.aspose.gridjs/gridjsworkbook\#CacheImp) .

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getGridLoadFormat(String extension) {#getGridLoadFormat-java.lang.String-}
```
public static int getGridLoadFormat(String extension)
```


Ottiene il formato di caricamento dall'estensione del file

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| extension | java.lang.String | L'estensione del file, di solito inizia con '.' . |

**Returns:**
int - [GridLoadFormat](../../com.aspose.gridjs/gridloadformat).
### getImageStream(String uid, String picid, String cachedir) {#getImageStream-java.lang.String-java.lang.String-java.lang.String-}
```
public static InputStream getImageStream(String uid, String picid, String cachedir)
```


Ottieni lo stream dell'immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'id univoco per la cache del file. |
| picid | java.lang.String | L'ID dell'immagine. |
| cachedir | java.lang.String |  |

**Returns:**
java.io.InputStream - Il flusso dell'immagine
### getImageUrl(String uid, String picid, String delimiter) {#getImageUrl-java.lang.String-java.lang.String-java.lang.String-}
```
public static String getImageUrl(String uid, String picid, String delimiter)
```


Ottiene l'URL dell'immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'id univoco per la cache del file. |
| picid | java.lang.String | L'ID dell'immagine. |
| delimiter | java.lang.String | Il delimitatore di stringa. |

**Returns:**
java.lang.String -
### getJsonByUid(String uid, String filename) {#getJsonByUid-java.lang.String-java.lang.String-}
```
public StringBuilder getJsonByUid(String uid, String filename)
```


Ottiene la stringa JSON del file dalla cache usando l'ID univoco specificato, imposta il nome file di output nel JSON.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'id univoco per la cache del file. |
| nome file | java.lang.String | Specifica il nome del file nel JSON. Se impostato a null, il nome file predefinito è: book1. |

**Returns:**
java.lang.StringBuilder - Il StringBuilder di stringa JSON
### getOle(String uid, String sheetname, int oleid, String label) {#getOle-java.lang.String-java.lang.String-int-java.lang.String-}
```
public byte[] getOle(String uid, String sheetname, int oleid, String label)
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
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Rappresenta le impostazioni della cartella di lavoro.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings)
### getSheetJsonWithCache(String uid, String sheetName, String fileName) {#getSheetJsonWithCache-java.lang.String-java.lang.String-java.lang.String-}
```
public String getSheetJsonWithCache(String uid, String sheetName, String fileName)
```


\\u947e\\u5cf0\\u5f47\\u93b8\\u56e7\\u757e foglio \\u9428?JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b?\*

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |
| sheetName | java.lang.String | \\u5bb8\\u30e4\\u7d94\\u741b\\u3125\\u6095\\u7ec9?\* @param fileName \\u9358\\u71b7\\ue750\\u93c2\\u56e6\\u6b22\\u935a?\* @return JSON \\u701b\\u6943\\ue0c1\\u6d93? |
| fileName | java.lang.String |  |

**Returns:**
java.lang.String
### getUidForFile(String fileName) {#getUidForFile-java.lang.String-}
```
public static String getUidForFile(String fileName)
```


Genera un nuovo ID univoco per la cache dei file utilizzando il nome file fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome del file. |

**Returns:**
java.lang.String -
### getWorkbookJsonWithCache(String uid, String fileName) {#getWorkbookJsonWithCache-java.lang.String-java.lang.String-}
```
public String getWorkbookJsonWithCache(String uid, String fileName)
```


\\u947e\\u5cf0\\u5f47\\u93c1\\u7fe0\\u91dc\\u5bb8\\u30e4\\u7d94\\u7ee8\\u8de8\\u6b91 JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b?\*

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |
| fileName | java.lang.String | \\u9358\\u71b7\\ue750\\u93c2\\u56e6\\u6b22\\u935a?\* @return JSON \\u701b\\u6943\\ue0c1\\u6d93? |

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importExcelFile(InputStream filestream, int format) {#importExcelFile-java.io.InputStream-int-}
```
public void importExcelFile(InputStream filestream, int format)
```


Importa il file Excel dallo stream del file con il formato di caricamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filestream | java.io.InputStream | Il flusso del file Excel. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). Il LoadFormat del file Excel. |

### importExcelFile(InputStream filestream, int format, String password) {#importExcelFile-java.io.InputStream-int-java.lang.String-}
```
public void importExcelFile(InputStream filestream, int format, String password)
```


Importa il file Excel dallo stream del file con il formato di caricamento e password di apertura.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filestream | java.io.InputStream | Il flusso del file Excel. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). Il LoadFormat del file Excel. |
| password | java.lang.String | La password di apertura del file Excel. Il valore può essere null se non è impostata alcuna password. |

### importExcelFile(String fileName) {#importExcelFile-java.lang.String-}
```
public void importExcelFile(String fileName)
```


Importa il file Excel dal percorso del file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il percorso completo del file. |

### importExcelFile(String uid, InputStream filestream, int format) {#importExcelFile-java.lang.String-java.io.InputStream-int-}
```
public void importExcelFile(String uid, InputStream filestream, int format)
```


Importa il file Excel dallo stream del file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'ID univoco per la cache del file, se impostato a null, verrà generato automaticamente. |
| filestream | java.io.InputStream | Il flusso del file Excel. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). Il LoadFormat del file Excel. |

### importExcelFile(String uid, InputStream filestream, int format, String password) {#importExcelFile-java.lang.String-java.io.InputStream-int-java.lang.String-}
```
public void importExcelFile(String uid, InputStream filestream, int format, String password)
```


Importa il file Excel dallo stream del file con il formato di caricamento e password di apertura.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'ID univoco per la cache del file, se impostato a null, verrà generato automaticamente. |
| filestream | java.io.InputStream | Il flusso del file Excel. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). Il LoadFormat del file Excel. |
| password | java.lang.String | La password di apertura del file Excel. Il valore può essere null se non è impostata alcuna password. |

### importExcelFile(String uid, String fileName) {#importExcelFile-java.lang.String-java.lang.String-}
```
public void importExcelFile(String uid, String fileName)
```


Importa il file Excel dal percorso del file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'ID univoco per la cache del file, se impostato a null, verrà generato automaticamente. |
| fileName | java.lang.String | Il percorso completo del file. |

### importExcelFile(String uid, String fileName, String password) {#importExcelFile-java.lang.String-java.lang.String-java.lang.String-}
```
public void importExcelFile(String uid, String fileName, String password)
```


Importa il file Excel dal percorso del file e password di apertura.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'ID univoco per la cache del file, se impostato a null, verrà generato automaticamente. |
| fileName | java.lang.String | Il percorso completo del file. |
| password | java.lang.String | La password di apertura del file Excel. Il valore può essere null se non è impostata alcuna password. |

### importExcelFileFromJson(String json) {#importExcelFileFromJson-java.lang.String-}
```
public void importExcelFileFromJson(String json)
```


Importa il file Excel da una stringa in formato JSON.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| json | java.lang.String | La stringa di formato JSON. |

### insertImage(String uid, String p, InputStream s, String imageUrl) {#insertImage-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-}
```
public String insertImage(String uid, String p, InputStream s, String imageUrl)
```


Inserisce un'immagine nel foglio di lavoro dallo stream del file o dall'URL (deve essere fornito lo stream del file o l'URL) oppure inserisce una forma, quando p.type è uno di AutoShapeType

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'ID univoco per la cache del file |
| p | java.lang.String | La stringa di formato JSON per l'operazione che specifica la posizione della cella, il nome del foglio di lavoro, la riga in alto a sinistra, la colonna in alto a sinistra per l'immagine\\u951b\\u5b94tc \{name:'sheet1',ri:1,ci:1\} |
| s | java.io.InputStream | Il flusso del file immagine |
| imageUrl | java.lang.String | L'URL del file immagine |

**Returns:**
java.lang.String - La stringa di formato JSON dell'immagine inserita
### jsonToStream(OutputStream stream, String filename) {#jsonToStream-java.io.OutputStream-java.lang.String-}
```
public void jsonToStream(OutputStream stream, String filename)
```


Genera JSON dal Workbook in memoria e lo scrive nello stream specificato. Opzionalmente memorizza nella cache il JSON generato per un recupero successivo più veloce. Differenze principali rispetto a JsonToStreamByUid: - Questo metodo utilizza lo stato corrente del Workbook in memoria (campo wb) - JsonToStreamByUid ricarica il Workbook dai file di cache .cells su disco - Usa questo metodo quando vuoi esportare lo stato corrente del workbook dopo le modifiche - Usa JsonToStreamByUid quando è necessario rigenerare JSON da uno stato di file precedentemente memorizzato nella cache. Comportamento della cache (quando uid è fornito): - Controlla la cache JSON prima di generare (L1 memoria + L2 disco) - In caso di cache miss, genera JSON dal workbook in memoria - Memorizza il JSON generato nella cache per richieste future

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Lo stream di output su cui scrivere i dati JSON |
| nome file | java.lang.String | Specifica il nome del file nel JSON. Se impostato a null, il nome file predefinito è: book1. |

### jsonToStream(OutputStream stream, String filename, String uid) {#jsonToStream-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void jsonToStream(OutputStream stream, String filename, String uid)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream |  |
| nome file | java.lang.String |  |
| uid | java.lang.String |  |

### jsonToStreamByUid(OutputStream stream, String uid, String filename) {#jsonToStreamByUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public boolean jsonToStreamByUid(OutputStream stream, String uid, String filename)
```


Recupera la stringa JSON del file dalla cache usando l'ID univoco specificato, imposta il nome file di output nel JSON e lo scrive nello stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso che verrà scritto |
| uid | java.lang.String | L'id univoco per la cache del file. |
| nome file | java.lang.String | Specifica il nome del file nel JSON. Se impostato a null, il nome file predefinito è: book1. |

**Returns:**
boolean
### lazyLoadingJson(String uid, String sheetName) {#lazyLoadingJson-java.lang.String-java.lang.String-}
```
public StringBuilder lazyLoadingJson(String uid, String sheetName)
```


Ottiene la stringa JSON del foglio specificato nel file dalla cache usando l'ID univoco specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'id univoco per la cache del file. |
| sheetName | java.lang.String | il nome del foglio. |

**Returns:**
java.lang.StringBuilder - Il StringBuilder di stringa JSON
### lazyLoadingStream(OutputStream stream, String uid, String sheetName) {#lazyLoadingStream-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void lazyLoadingStream(OutputStream stream, String uid, String sheetName)
```


Recupera la stringa JSON del foglio specificato nel file dalla cache usando l'ID univoco specificato e la scrive nello stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso che verrà scritto |
| uid | java.lang.String | L'id univoco per la cache del file. |
| sheetName | java.lang.String | il nome del foglio. |

### mergeExcelFileFromJson(String uid, String json) {#mergeExcelFileFromJson-java.lang.String-java.lang.String-}
```
public void mergeExcelFileFromJson(String uid, String json)
```


Applica un aggiornamento batch ai dati in memoria.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'id univoco per la cache del file. |
| json | java.lang.String | La stringa di formato JSON di aggiornamento. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr) {#redactFile-java.lang.String-java.lang.String-java.lang.String---}
```
public void redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr)
```


Esegue la redazione di un file Excel basata su un array di operazioni JSON.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| excelFilePath | java.lang.String | Il percorso del file Excel da redigere. |
| uid | java.lang.String | L'identificatore univoco per la cartella di lavoro. Se nullo o vuoto, verrà generato un nuovo uid basato sul percorso del file. |
| arrayOfRedactionOpr | java.lang.String[] | Un array di stringhe JSON che rappresentano le operazioni di redazione da applicare. |

### saveToCacheWithFileName(String uid, String filename, String password) {#saveToCacheWithFileName-java.lang.String-java.lang.String-java.lang.String-}
```
public void saveToCacheWithFileName(String uid, String filename, String password)
```


Salva i dati in memoria nel file di cache con il nome file specificato e imposta anche la password di apertura; il formato di salvataggio è basato sull'estensione del nome file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'id univoco per la cache del file. |
| nome file | java.lang.String | Il nome file da salvare. |
| password | java.lang.String | La password di apertura del file Excel. Il valore può essere null se non è impostata alcuna password. |

### saveToExcelFile(OutputStream stream) {#saveToExcelFile-java.io.OutputStream-}
```
public void saveToExcelFile(OutputStream stream)
```


Salva i dati in memoria nello sream, basato sul formato originale del file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso da salvare. |

### saveToExcelFile(String path) {#saveToExcelFile-java.lang.String-}
```
public void saveToExcelFile(String path)
```


Salva i dati in memoria nel percorso del file; se il file ha un'estensione, il formato di salvataggio è basato sull'estensione del file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | java.lang.String | Il percorso file dove salvare. |

### saveToHtml(OutputStream stream) {#saveToHtml-java.io.OutputStream-}
```
public void saveToHtml(OutputStream stream)
```


Salva i dati in memoria nello sream, il formato di salvataggio è html

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso da salvare. |

### saveToHtml(String path) {#saveToHtml-java.lang.String-}
```
public void saveToHtml(String path)
```


Salva i dati in memoria nel percorso del file, il formato di salvataggio è html.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | java.lang.String | Il percorso file dove salvare. |

### saveToPdf(OutputStream stream) {#saveToPdf-java.io.OutputStream-}
```
public void saveToPdf(OutputStream stream)
```


Salva i dati in memoria nello sream, il formato di salvataggio è pdf.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso da salvare. |

### saveToPdf(String path) {#saveToPdf-java.lang.String-}
```
public void saveToPdf(String path)
```


Salva i dati in memoria nel percorso file, il formato di salvataggio è pdf.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | java.lang.String | Il percorso file dove salvare. |

### saveToXlsx(OutputStream stream) {#saveToXlsx-java.io.OutputStream-}
```
public void saveToXlsx(OutputStream stream)
```


Salva i dati in memoria nello stream, il formato di salvataggio è xlsx.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso da salvare. |

### saveToXlsx(String path) {#saveToXlsx-java.lang.String-}
```
public void saveToXlsx(String path)
```


Salva i dati in memoria nel percorso file, il formato di salvataggio è xlsx.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | java.lang.String | Il percorso file dove salvare. |

### setCacheDirectory(String value) {#setCacheDirectory-java.lang.String-}
```
public void setCacheDirectory(String value)
```


Imposta la directory cache per la memorizzazione dei file di foglio di calcolo. Se non è impostata, utilizzeremo la proprietà statica da [Config.getFileCacheDirectory()](../../com.aspose.gridjs/config\#getFileCacheDirectory--) o [CacheImp](../../com.aspose.gridjs/gridjsworkbook\#CacheImp).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setImageUrlBase(String baseImageURL) {#setImageUrlBase-java.lang.String-}
```
public static void setImageUrlBase(String baseImageURL)
```


Imposta l'URL di azione per ottenere l'immagine di base dal controller.

**Remarks**

Quando CacheImp è null, dobbiamo impostare questo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| baseImageURL | java.lang.String | L'URL dell'azione di recupero dell'immagine di base. |

### setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds) {#setInterruptMonitorForLoad-com.aspose.gridjs.GridInterruptMonitor-int-}
```
public void setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds)
```


Imposta InterruptMonitor per l'operazione di caricamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| monitor | [GridInterruptMonitor](../../com.aspose.gridjs/gridinterruptmonitor) | L'istanza di InterruptMonitor. |
| calculateTimeoutMilliseconds | int | Il timeout in millisecondi per il caricamento del file. |

### setInterruptMonitorForSave(GridInterruptMonitor monitor) {#setInterruptMonitorForSave-com.aspose.gridjs.GridInterruptMonitor-}
```
public void setInterruptMonitorForSave(GridInterruptMonitor monitor)
```


Imposta InterruptMonitor per l'operazione di salvataggio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| monitor | [GridInterruptMonitor](../../com.aspose.gridjs/gridinterruptmonitor) | L'istanza di InterruptMonitor. |

### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridjs.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Rappresenta le impostazioni della cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings) |  |

### setTransParentView(String excelFilePath, String uid, boolean isTransparent) {#setTransParentView-java.lang.String-java.lang.String-boolean-}
```
public void setTransParentView(String excelFilePath, String uid, boolean isTransparent)
```


Imposta la trasparenza delle forme di redazione nella cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| excelFilePath | java.lang.String | Il percorso del file Excel. |
| uid | java.lang.String | L'identificatore univoco per la cartella di lavoro. Se nullo o vuoto, verrà generato un nuovo uid basato sul percorso del file. |
| isTransparent | boolean | Se true, imposta la trasparenza a 0.89 (semi-trasparente); se false, imposta la trasparenza a 1 (completamente opaco/invisibile). |

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
java.lang.String - La stringa in formato JSON del risultato dell'aggiornamento.
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

