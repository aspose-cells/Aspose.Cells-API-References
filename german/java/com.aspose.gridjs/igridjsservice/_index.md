---
title: "IGridJsService"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Schnittstelle für grundlegende Operations‑APIs dar, die in Controller‑Aktionen verwendet wird."
type: docs
url: /de/java/com.aspose.gridjs/igridjsservice/
---
```
public interface IGridJsService
```

Stellt die Schnittstelle für grundlegende Operations‑APIs dar, die in Controller‑Aktionen verwendet wird.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addImage(String p, String uid, InputStream filestream)](#addImage-java.lang.String-java.lang.String-java.io.InputStream-) | Wendet die Operation zum Hinzufügen eines Bildes aus einer lokalen Datei an. |
| [addImageByURL(String p, String uid, InputStream filestream, String imageurl)](#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Wendet die Operation zum Hinzufügen eines Bildes von einer Remote-URL an. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Überprüfen Sie, ob die Workbook-Instanz im Speicher-Cache ist. Diese Methode wird nur für den Collaborative‑Modus angewendet. |
| [clearAllJsonCache()](#clearAllJsonCache--) | Löscht alle JSON-Cache‑Einträge (Speicher und Festplatte). |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | Löscht alle JSON-Cache‑Einträge, die zur angegebenen eindeutigen ID gehören. |
| [copyImage(String p, String uid)](#copyImage-java.lang.String-java.lang.String-) | Führt die Kopier‑Bild‑Operation aus. |
| [detailFileJsonWithUid(String filePath, String uid)](#detailFileJsonWithUid-java.lang.String-java.lang.String-) | Liefert den JSON‑String für die Datei anhand der angegebenen eindeutigen ID. |
| [detailStreamJson(OutputStream stream, String filePath)](#detailStreamJson-java.io.OutputStream-java.lang.String-) | Schreibt die JSON-Zeichenfolge für die Arbeitsmappe in den Stream |
| [detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)](#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Schreibt den JSON‑String für die Datei in den Stream anhand der angegebenen eindeutigen ID. |
| [dispose()](#dispose--) |  |
| [download(String p, String uid, String filename)](#download-java.lang.String-java.lang.String-java.lang.String-) | Führt die Download‑Datei‑Operation aus |
| [getFile(String fileid)](#getFile-java.lang.String-) | Datei‑Stream abrufen |
| [image(String uid, String picid)](#image-java.lang.String-java.lang.String-) | Bild‑Stream abrufen. |
| [imageUrl(String baseURL, String picid, String uid)](#imageUrl-java.lang.String-java.lang.String-java.lang.String-) | Liefert die Bild‑URL. |
| [lazyLoadingJson(String sheetName, String uid)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Liefert den JSON‑String des angegebenen Tabellenblatts in der Datei aus dem Cache mittels der angegebenen eindeutigen ID. |
| [lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)](#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-) | Schreibt den JSON‑String des angegebenen Tabellenblatts in der Datei aus dem Cache mittels der angegebenen eindeutigen ID in den Stream. |
| [load(String uid, String filename)](#load-java.lang.String-java.lang.String-) | Liefert den JSON‑String der Datei aus dem Cache anhand der angegebenen eindeutigen ID, setzt den Ausgabedateinamen im JSON. |
| [ole(String uid, String sheetname, int oleid, String label)](#ole-java.lang.String-java.lang.String-int-java.lang.String-) | Liefert die Byte‑Array‑Daten des eingebetteten OLE‑Objekts. |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Führt die Update‑Operation aus. |
### addImage(String p, String uid, InputStream filestream) {#addImage-java.lang.String-java.lang.String-java.io.InputStream-}
```
public abstract String addImage(String p, String uid, InputStream filestream)
```


Wendet die Operation zum Hinzufügen eines Bildes aus einer lokalen Datei an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| p | java.lang.String | Der JSON‑String‑Parameter |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |
| filestream | java.io.InputStream | Der Filestream des Bildes |

**Returns:**
java.lang.String - Das JSON‑String‑Ergebnis
### addImageByURL(String p, String uid, InputStream filestream, String imageurl) {#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-}
```
public abstract String addImageByURL(String p, String uid, InputStream filestream, String imageurl)
```


Wendet die Operation zum Hinzufügen eines Bildes von einer Remote-URL an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| p | java.lang.String | Der JSON‑String‑Parameter |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |
| filestream | java.io.InputStream | Der Filestream des Bildes |
| imageurl | java.lang.String | Geben Sie die Bild‑URL an. |

**Returns:**
java.lang.String - Das JSON‑String‑Ergebnis
### checkInCacheForCollaborative(String uid) {#checkInCacheForCollaborative-java.lang.String-}
```
public abstract boolean checkInCacheForCollaborative(String uid)
```


Überprüfen Sie, ob die Workbook-Instanz im Speicher-Cache ist. Diese Methode wird nur für den Collaborative‑Modus angewendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String |  |

**Returns:**
boolean -
### clearAllJsonCache() {#clearAllJsonCache--}
```
public abstract void clearAllJsonCache()
```


Löscht alle JSON-Cache‑Einträge (Speicher und Festplatte).

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public abstract void clearJsonCacheForUid(String uid)
```


Löscht alle JSON-Cache-Einträge, die zur angegebenen eindeutigen ID gehören. Rufen Sie dies auf, nachdem Sie die Quelldatei außerhalb des normalen Ablaufs geändert haben, damit die nächste Anforderung das JSON neu generiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |

### copyImage(String p, String uid) {#copyImage-java.lang.String-java.lang.String-}
```
public abstract String copyImage(String p, String uid)
```


Führt die Kopier‑Bild‑Operation aus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| p | java.lang.String | Der JSON‑String‑Parameter |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |

**Returns:**
java.lang.String - Das JSON‑String‑Ergebnis
### detailFileJsonWithUid(String filePath, String uid) {#detailFileJsonWithUid-java.lang.String-java.lang.String-}
```
public abstract StringBuilder detailFileJsonWithUid(String filePath, String uid)
```


Liefert den JSON‑String für die Datei anhand der angegebenen eindeutigen ID.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Der Dateipfad |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |

**Returns:**
java.lang.StringBuilder
### detailStreamJson(OutputStream stream, String filePath) {#detailStreamJson-java.io.OutputStream-java.lang.String-}
```
public abstract void detailStreamJson(OutputStream stream, String filePath)
```


Schreibt die JSON-Zeichenfolge für die Arbeitsmappe in den Stream

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Stream, der geschrieben wird |
| filePath | java.lang.String | Der Dateipfad |

### detailStreamJsonWithUid(OutputStream stream, String filePath, String uid) {#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public abstract void detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)
```


Schreibt den JSON‑String für die Datei in den Stream anhand der angegebenen eindeutigen ID.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Stream, der geschrieben wird |
| filePath | java.lang.String | Der Dateipfad |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |

### dispose() {#dispose--}
```
public abstract void dispose()
```




### download(String p, String uid, String filename) {#download-java.lang.String-java.lang.String-java.lang.String-}
```
public abstract String download(String p, String uid, String filename)
```


Führt die Download‑Datei‑Operation aus

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| p | java.lang.String | Der JSON-Parameter |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |
| Dateiname | java.lang.String | Der Dateiname |

**Returns:**
java.lang.String - Die Datei-URL
### getFile(String fileid) {#getFile-java.lang.String-}
```
public abstract InputStream getFile(String fileid)
```


Datei‑Stream abrufen

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileid | java.lang.String | die Datei-ID |

**Returns:**
java.io.InputStream - Der Stream der Datei
### image(String uid, String picid) {#image-java.lang.String-java.lang.String-}
```
public abstract InputStream image(String uid, String picid)
```


Bild‑Stream abrufen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |
| picid | java.lang.String | Die Bild-ID. |

**Returns:**
java.io.InputStream - Der Bild-Stream
### imageUrl(String baseURL, String picid, String uid) {#imageUrl-java.lang.String-java.lang.String-java.lang.String-}
```
public abstract String imageUrl(String baseURL, String picid, String uid)
```


Liefert die Bild‑URL.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| baseURL | java.lang.String | Die Basis-Aktions-URL. |
| picid | java.lang.String | Die Bild-ID. |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |

**Returns:**
java.lang.String - Die Bild-URL
### lazyLoadingJson(String sheetName, String uid) {#lazyLoadingJson-java.lang.String-java.lang.String-}
```
public abstract StringBuilder lazyLoadingJson(String sheetName, String uid)
```


Liefert den JSON‑String des angegebenen Tabellenblatts in der Datei aus dem Cache mittels der angegebenen eindeutigen ID.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetName | java.lang.String | der Blattname. |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |

**Returns:**
java.lang.StringBuilder
### lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid) {#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public abstract void lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)
```


Schreibt den JSON‑String des angegebenen Tabellenblatts in der Datei aus dem Cache mittels der angegebenen eindeutigen ID in den Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Stream, der geschrieben wird |
| sheetName | java.lang.String | Der Blattname. |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |

### load(String uid, String filename) {#load-java.lang.String-java.lang.String-}
```
public abstract String load(String uid, String filename)
```


Liefert den JSON‑String der Datei aus dem Cache anhand der angegebenen eindeutigen ID, setzt den Ausgabedateinamen im JSON.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |
| Dateiname | java.lang.String | Gibt den Dateinamen im JSON an. Wenn er auf null gesetzt wird, ist der Standarddateiname: book1. |

**Returns:**
java.lang.String - Der JSON-String
### ole(String uid, String sheetname, int oleid, String label) {#ole-java.lang.String-java.lang.String-int-java.lang.String-}
```
public abstract byte[] ole(String uid, String sheetname, int oleid, String label)
```


Liefert die Byte‑Array‑Daten des eingebetteten OLE‑Objekts.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |
| sheetname | java.lang.String | Der Arbeitsblattname. |
| oleid | int | Die ID für das eingebettete OLE-Objekt. |
| label | java.lang.String | Das Anzeigetext des eingebetteten OLE-Objekts. |

**Returns:**
byte[] - Die Byte-Array-Daten des eingebetteten OLE-Objekts.
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public abstract String updateCell(String p, String uid)
```


Führt die Update‑Operation aus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| p | java.lang.String | Der JSON-Format-String der Aktualisierungsoperation. |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |

**Returns:**
java.lang.String
