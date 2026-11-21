---
title: "IGridJsService"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar det grundläggande operations‑API‑gränssnittet som används i kontrolleråtgärder."
type: docs
url: /sv/java/com.aspose.gridjs/igridjsservice/
---
```
public interface IGridJsService
```

Representerar det grundläggande operations‑API‑gränssnittet som används i kontrolleråtgärder.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addImage(String p, String uid, InputStream filestream)](#addImage-java.lang.String-java.lang.String-java.io.InputStream-) | Tillämpar operationen att lägga till bild från lokal fil. |
| [addImageByURL(String p, String uid, InputStream filestream, String imageurl)](#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Tillämpar operationen för att lägga till bild från fjärr-URL. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Kontrollera om arbetsboksinstansen finns i minnescachen. Denna metod gäller endast för samarbetsläge. |
| [clearAllJsonCache()](#clearAllJsonCache--) | Rensar alla JSON-cacheposter (minne och disk). |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | Rensar alla JSON-cacheposter som tillhör det angivna unika ID:t. |
| [copyImage(String p, String uid)](#copyImage-java.lang.String-java.lang.String-) | Tillämpar kopieringsoperationen för bild. |
| [detailFileJsonWithUid(String filePath, String uid)](#detailFileJsonWithUid-java.lang.String-java.lang.String-) | Hämtar JSON-sträng för filen med det angivna unika ID:t. |
| [detailStreamJson(OutputStream stream, String filePath)](#detailStreamJson-java.io.OutputStream-java.lang.String-) | Skriv JSON-strängen för arbetsboken till strömmen |
| [detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)](#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Skriv JSON-strängen för filen till strömmen med det angivna unika ID:t. |
| [dispose()](#dispose--) |  |
| [download(String p, String uid, String filename)](#download-java.lang.String-java.lang.String-java.lang.String-) | Tillämpar nedladdningsoperationen för filen |
| [getFile(String fileid)](#getFile-java.lang.String-) | Hämta filström |
| [image(String uid, String picid)](#image-java.lang.String-java.lang.String-) | Hämta ström av bild. |
| [imageUrl(String baseURL, String picid, String uid)](#imageUrl-java.lang.String-java.lang.String-java.lang.String-) | Hämtar bildens URL. |
| [lazyLoadingJson(String sheetName, String uid)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Hämtar JSON-strängen för det angivna bladet i filen från cachen med den angivna unika ID:n. |
| [lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)](#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-) | Skriver JSON-strängen för det angivna bladet i filen från cachen med den angivna unika ID:n till strömmen. |
| [load(String uid, String filename)](#load-java.lang.String-java.lang.String-) | Hämtar JSON-strängen för filen från cachen med den angivna unika ID:n, sätter utdatafilnamnet i JSON. |
| [ole(String uid, String sheetname, int oleid, String label)](#ole-java.lang.String-java.lang.String-int-java.lang.String-) | Hämtar bytearray-data för det inbäddade OLE-objektet. |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Tillämpar uppdateringsoperationen. |
### addImage(String p, String uid, InputStream filestream) {#addImage-java.lang.String-java.lang.String-java.io.InputStream-}
```
public abstract String addImage(String p, String uid, InputStream filestream)
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
public abstract String addImageByURL(String p, String uid, InputStream filestream, String imageurl)
```


Tillämpar operationen för att lägga till bild från fjärr-URL.

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
public abstract boolean checkInCacheForCollaborative(String uid)
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
public abstract void clearAllJsonCache()
```


Rensar alla JSON-cacheposter (minne och disk).

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public abstract void clearJsonCacheForUid(String uid)
```


Rensar alla JSON-cacheposter som tillhör den angivna unika ID:n. Anropa detta efter att ha ändrat källfilen externt så att nästa begäran genererar JSON igen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika id-et för filcachen. |

### copyImage(String p, String uid) {#copyImage-java.lang.String-java.lang.String-}
```
public abstract String copyImage(String p, String uid)
```


Tillämpar kopieringsoperationen för bild.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| p | java.lang.String | JSON-strängparameter |
| uid | java.lang.String | Det unika id-et för filcachen. |

**Returns:**
java.lang.String - JSON-strängresultat
### detailFileJsonWithUid(String filePath, String uid) {#detailFileJsonWithUid-java.lang.String-java.lang.String-}
```
public abstract StringBuilder detailFileJsonWithUid(String filePath, String uid)
```


Hämtar JSON-sträng för filen med det angivna unika ID:t.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | Filens sökväg |
| uid | java.lang.String | Det unika id-et för filcachen. |

**Returns:**
java.lang.StringBuilder
### detailStreamJson(OutputStream stream, String filePath) {#detailStreamJson-java.io.OutputStream-java.lang.String-}
```
public abstract void detailStreamJson(OutputStream stream, String filePath)
```


Skriv JSON-strängen för arbetsboken till strömmen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Strömmen som kommer att skrivas |
| filePath | java.lang.String | Filens sökväg |

### detailStreamJsonWithUid(OutputStream stream, String filePath, String uid) {#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public abstract void detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)
```


Skriv JSON-strängen för filen till strömmen med det angivna unika ID:t.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Strömmen som kommer att skrivas |
| filePath | java.lang.String | Filens sökväg |
| uid | java.lang.String | Det unika id-et för filcachen. |

### dispose() {#dispose--}
```
public abstract void dispose()
```




### download(String p, String uid, String filename) {#download-java.lang.String-java.lang.String-java.lang.String-}
```
public abstract String download(String p, String uid, String filename)
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
### getFile(String fileid) {#getFile-java.lang.String-}
```
public abstract InputStream getFile(String fileid)
```


Hämta filström

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileid | java.lang.String | filens ID |

**Returns:**
java.io.InputStream - Strömmen av filen
### image(String uid, String picid) {#image-java.lang.String-java.lang.String-}
```
public abstract InputStream image(String uid, String picid)
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
public abstract String imageUrl(String baseURL, String picid, String uid)
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
public abstract StringBuilder lazyLoadingJson(String sheetName, String uid)
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
public abstract void lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)
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
public abstract String load(String uid, String filename)
```


Hämtar JSON-strängen för filen från cachen med den angivna unika ID:n, sätter utdatafilnamnet i JSON.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika id-et för filcachen. |
| filnamn | java.lang.String | Anger filnamnet i JSON. Om den sätts till null, är standardfilnamnet: book1. |

**Returns:**
java.lang.String - JSON-strängen
### ole(String uid, String sheetname, int oleid, String label) {#ole-java.lang.String-java.lang.String-int-java.lang.String-}
```
public abstract byte[] ole(String uid, String sheetname, int oleid, String label)
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
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public abstract String updateCell(String p, String uid)
```


Tillämpar uppdateringsoperationen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| p | java.lang.String | JSON-formatsträngen för uppdateringsoperationen. |
| uid | java.lang.String | Det unika id-et för filcachen. |

**Returns:**
java.lang.String
