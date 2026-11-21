---
title: "GridJsService"
second_title: "Aspose.Cells för Java API-referens"
description: "Tillhandahåller de grundläggande operations‑API:erna som används i kontrolleråtgärder."
type: docs
url: /sv/java/com.aspose.gridjs/gridjsservice/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.gridjs.IGridJsService](../../com.aspose.gridjs/igridjsservice)
```
public class GridJsService implements IGridJsService
```

Tillhandahåller de grundläggande operations‑API:erna som används i kontrolleråtgärder.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [GridJsService(GridJsOptions options)](#GridJsService-com.aspose.gridjs.GridJsOptions-) | Standardkonstruktorn för GridJsService |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addImage(String p, String uid, InputStream filestream)](#addImage-java.lang.String-java.lang.String-java.io.InputStream-) | Tillämpar operationen att lägga till bild från lokal fil. |
| [addImageByURL(String p, String uid, InputStream filestream, String imageurl)](#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Tillämpar operationen att lägga till bild från lokal fil. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Kontrollera om arbetsboksinstansen finns i minnescachen. Denna metod gäller endast för samarbetsläge. |
| [clearAllJsonCache()](#clearAllJsonCache--) | Rensar alla JSON-cacheposter (minne och disk). |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | Rensar alla JSON-cacheposter som tillhör det angivna unika ID:t. |
| [copyImage(String p, String uid)](#copyImage-java.lang.String-java.lang.String-) | Tillämpar kopieringsoperationen för bild. |
| [destroy()](#destroy--) | Denna metod är endast för Java, den implementerar destroy-metoden i DisposableBean, som kommer att anropas automatiskt av Spring när begäran avslutas, i själva verket kommer den att anropa Dispose-metoden. |
| [detailFileJsonWithUid(String filePath, String uid)](#detailFileJsonWithUid-java.lang.String-java.lang.String-) | Hämtar JSON-sträng för filen med det angivna unika ID:t. |
| [detailStreamJson(OutputStream stream, String filePath)](#detailStreamJson-java.io.OutputStream-java.lang.String-) | Skriv JSON-strängen för filen till strömmen. |
| [detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)](#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Skriv JSON-strängen för filen till strömmen med det angivna unika ID:t. |
| [dispose()](#dispose--) | Utför applikationsdefinierade uppgifter som är relaterade till att frigöra, släppa eller återställa ohanterade resurser. |
| [download(String p, String uid, String filename)](#download-java.lang.String-java.lang.String-java.lang.String-) | Tillämpar nedladdningsoperationen för filen |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFile(String fileid)](#getFile-java.lang.String-) | Hämta filström |
| [getSettings()](#getSettings--) | Representerar arbetsbokens inställningar. |
| [hashCode()](#hashCode--) |  |
| [image(String uid, String picid)](#image-java.lang.String-java.lang.String-) | Hämta ström av bild. |
| [imageUrl(String baseURL, String picid, String uid)](#imageUrl-java.lang.String-java.lang.String-java.lang.String-) | Hämtar bildens URL. |
| [lazyLoadingJson(String sheetName, String uid)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Hämtar JSON-strängen för det angivna bladet i filen från cachen med den angivna unika ID:n. |
| [lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)](#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-) | Skriver JSON-strängen för det angivna bladet i filen från cachen med den angivna unika ID:n till strömmen. |
| [load(String uid, String filename)](#load-java.lang.String-java.lang.String-) | Hämtar JSON-strängen för filen från cachen med den angivna unika ID:n, sätter utdatafilnamnet i JSON. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [ole(String uid, String sheetname, int oleid, String label)](#ole-java.lang.String-java.lang.String-int-java.lang.String-) | Hämtar bytearray-data för det inbäddade OLE-objektet. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridjs.GridWorkbookSettings-) | Representerar arbetsbokens inställningar. |
| [toString()](#toString--) |  |
| [translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)](#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-) | Översätt alla strängvärden till målspråket i kalkylbladet. |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Tillämpar uppdateringsoperationen. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsService(GridJsOptions options) {#GridJsService-com.aspose.gridjs.GridJsOptions-}
```
public GridJsService(GridJsOptions options)
```


Standardkonstruktorn för GridJsService

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | [GridJsOptions](../../com.aspose.gridjs/gridjsoptions) |  |

### addImage(String p, String uid, InputStream filestream) {#addImage-java.lang.String-java.lang.String-java.io.InputStream-}
```
public String addImage(String p, String uid, InputStream filestream)
```


Tillämpar operationen att lägga till bild från lokal fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| p | java.lang.String | JSON-strängparameter |
| uid | java.lang.String | Det unika id-et för filcachen. |
| filestream | java.io.InputStream | filestream för bilden |

**Returns:**
java.lang.String - JSON-strängresultat
### addImageByURL(String p, String uid, InputStream filestream, String imageurl) {#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-}
```
public String addImageByURL(String p, String uid, InputStream filestream, String imageurl)
```


Tillämpar operationen att lägga till bild från lokal fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| p | java.lang.String | JSON-strängparameter |
| uid | java.lang.String | Det unika id-et för filcachen. |
| filestream | java.io.InputStream | filestream för bilden |
| imageurl | java.lang.String | Ange bildens URL. |

**Returns:**
java.lang.String - JSON-strängresultat
### checkInCacheForCollaborative(String uid) {#checkInCacheForCollaborative-java.lang.String-}
```
public boolean checkInCacheForCollaborative(String uid)
```


Kontrollera om arbetsboksinstansen finns i minnescachen. Denna metod gäller endast för samarbetsläge.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String |  |

**Returns:**
boolean -
### clearAllJsonCache() {#clearAllJsonCache--}
```
public void clearAllJsonCache()
```


Rensar alla JSON-cacheposter (minne och disk).

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public void clearJsonCacheForUid(String uid)
```


Rensar alla JSON-cacheposter som tillhör den angivna unika ID:n. Anropa detta efter att ha ändrat källfilen externt så att nästa begäran genererar JSON igen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika id-et för filcachen. |

### copyImage(String p, String uid) {#copyImage-java.lang.String-java.lang.String-}
```
public String copyImage(String p, String uid)
```


Tillämpar kopieringsoperationen för bild.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| p | java.lang.String | JSON-strängparameter |
| uid | java.lang.String | Det unika id-et för filcachen. |

**Returns:**
java.lang.String - JSON-strängresultat
### destroy() {#destroy--}
```
public void destroy()
```


Denna metod är endast för Java, den implementerar destroy-metoden i DisposableBean, som kommer att anropas automatiskt av Spring när begäran avslutas, i själva verket kommer den att anropa Dispose-metoden.

### detailFileJsonWithUid(String filePath, String uid) {#detailFileJsonWithUid-java.lang.String-java.lang.String-}
```
public StringBuilder detailFileJsonWithUid(String filePath, String uid)
```


Hämtar JSON-sträng för filen med det angivna unika ID:t.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | Den fullständiga filsökvägen |
| uid | java.lang.String | Det unika id-et för filcachen. |

**Returns:**
java.lang.StringBuilder
### detailStreamJson(OutputStream stream, String filePath) {#detailStreamJson-java.io.OutputStream-java.lang.String-}
```
public void detailStreamJson(OutputStream stream, String filePath)
```


Skriv JSON-strängen för filen till strömmen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Strömmen som kommer att skrivas |
| filePath | java.lang.String | Den fullständiga filsökvägen |

### detailStreamJsonWithUid(OutputStream stream, String filePath, String uid) {#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)
```


Skriv JSON-strängen för filen till strömmen med det angivna unika ID:t.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Strömmen som kommer att skrivas |
| filePath | java.lang.String | Den fullständiga filsökvägen |
| uid | java.lang.String | Det unika id-et för filcachen. |

### dispose() {#dispose--}
```
public void dispose()
```


Utför applikationsdefinierade uppgifter som är relaterade till att frigöra, släppa eller återställa ohanterade resurser.

### download(String p, String uid, String filename) {#download-java.lang.String-java.lang.String-java.lang.String-}
```
public String download(String p, String uid, String filename)
```


Tillämpar nedladdningsoperationen för filen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| p | java.lang.String | JSON-parameter |
| uid | java.lang.String | Det unika id-et för filcachen. |
| filnamn | java.lang.String | Filnamnet |

**Returns:**
java.lang.String - Filens URL
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
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


Hämta filström

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileid | java.lang.String | filens ID |

**Returns:**
java.io.InputStream - Strömmen av filen
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Representerar arbetsbokens inställningar.

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


Hämta ström av bild.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika id-et för filcachen. |
| picid | java.lang.String | Bildens id. |

**Returns:**
java.io.InputStream - Bildströmmen
### imageUrl(String baseURL, String picid, String uid) {#imageUrl-java.lang.String-java.lang.String-java.lang.String-}
```
public String imageUrl(String baseURL, String picid, String uid)
```


Hämtar bildens URL.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| baseURL | java.lang.String | Den grundläggande åtgärds-URL:en. |
| picid | java.lang.String | Bildens id. |
| uid | java.lang.String | Det unika id-et för filcachen. |

**Returns:**
java.lang.String - JSON-strängen
### lazyLoadingJson(String sheetName, String uid) {#lazyLoadingJson-java.lang.String-java.lang.String-}
```
public StringBuilder lazyLoadingJson(String sheetName, String uid)
```


Hämtar JSON-strängen för det angivna bladet i filen från cachen med den angivna unika ID:n.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetName | java.lang.String | bladnamnet. |
| uid | java.lang.String | Det unika id-et för filcachen. |

**Returns:**
java.lang.StringBuilder
### lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid) {#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)
```


Skriver JSON-strängen för det angivna bladet i filen från cachen med den angivna unika ID:n till strömmen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Strömmen som kommer att skrivas |
| sheetName | java.lang.String | Bladnamnet. |
| uid | java.lang.String | Det unika id-et för filcachen. |

### load(String uid, String filename) {#load-java.lang.String-java.lang.String-}
```
public String load(String uid, String filename)
```


Hämtar JSON-strängen för filen från cachen med den angivna unika ID:n, sätter utdatafilnamnet i JSON.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika id-et för filcachen. |
| filnamn | java.lang.String | Anger filnamnet i JSON. Om den sätts till null, är standardfilnamnet: book1. |

**Returns:**
java.lang.String - JSON-strängen
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


Hämtar bytearray-data för det inbäddade OLE-objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika id-et för filcachen. |
| sheetname | java.lang.String | Arbetsbladets namn. |
| oleid | int | ID för det inbäddade ole-objektet. |
| label | java.lang.String | Visningsetiketten för det inbäddade ole-objektet. |

**Returns:**
byte[] - Bytearraydata för det inbäddade ole-objektet.
### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridjs.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Representerar arbetsbokens inställningar.

**Parameters:**
| Parameter | Typ | Beskrivning |
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


Översätt alla strängvärden till målspråket i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika id-et för filcachen. |
| sheetName | java.lang.String | Bladnamnet |
| translator | [ITextTranslator](../../com.aspose.gridjs/itexttranslator) | Översättaren som implementerar översättningsfunktionen |
| targetLanguage | java.lang.String | Målspråket |

**Returns:**
java.lang.String -
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public String updateCell(String p, String uid)
```


Tillämpar uppdateringsoperationen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| p | java.lang.String | JSON-formatsträngen för uppdateringsoperationen. |
| uid | java.lang.String | Det unika id-et för filcachen. |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

