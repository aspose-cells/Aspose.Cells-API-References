---
title: "GridJsService"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die grundlegenden Operations‑APIs bereit, die in Controller‑Aktionen verwendet werden."
type: docs
url: /de/java/com.aspose.gridjs/gridjsservice/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.gridjs.IGridJsService](../../com.aspose.gridjs/igridjsservice)
```
public class GridJsService implements IGridJsService
```

Stellt die grundlegenden Operations‑APIs bereit, die in Controller‑Aktionen verwendet werden.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [GridJsService(GridJsOptions options)](#GridJsService-com.aspose.gridjs.GridJsOptions-) | Der Standardkonstruktor für GridJsService |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addImage(String p, String uid, InputStream filestream)](#addImage-java.lang.String-java.lang.String-java.io.InputStream-) | Wendet die Operation zum Hinzufügen eines Bildes aus einer lokalen Datei an. |
| [addImageByURL(String p, String uid, InputStream filestream, String imageurl)](#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Wendet die Operation zum Hinzufügen eines Bildes aus einer lokalen Datei an. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Überprüfen Sie, ob die Workbook-Instanz im Speicher-Cache ist. Diese Methode wird nur für den Collaborative‑Modus angewendet. |
| [clearAllJsonCache()](#clearAllJsonCache--) | Löscht alle JSON-Cache‑Einträge (Speicher und Festplatte). |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | Löscht alle JSON-Cache‑Einträge, die zur angegebenen eindeutigen ID gehören. |
| [copyImage(String p, String uid)](#copyImage-java.lang.String-java.lang.String-) | Führt die Kopier‑Bild‑Operation aus. |
| [destroy()](#destroy--) | Diese Methode ist nur für Java vorgesehen, sie implementiert die destroy‑Methode in DisposableBean, die von Spring automatisch aufgerufen wird, wenn die Anfrage abgeschlossen ist; tatsächlich ruft sie die Dispose‑Methode auf. |
| [detailFileJsonWithUid(String filePath, String uid)](#detailFileJsonWithUid-java.lang.String-java.lang.String-) | Liefert den JSON‑String für die Datei anhand der angegebenen eindeutigen ID. |
| [detailStreamJson(OutputStream stream, String filePath)](#detailStreamJson-java.io.OutputStream-java.lang.String-) | Schreibt den JSON‑String für die Datei in den Stream. |
| [detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)](#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Schreibt den JSON‑String für die Datei in den Stream anhand der angegebenen eindeutigen ID. |
| [dispose()](#dispose--) | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [download(String p, String uid, String filename)](#download-java.lang.String-java.lang.String-java.lang.String-) | Führt die Download‑Datei‑Operation aus |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFile(String fileid)](#getFile-java.lang.String-) | Datei‑Stream abrufen |
| [getSettings()](#getSettings--) | Stellt die Arbeitsmappeneinstellungen dar. |
| [hashCode()](#hashCode--) |  |
| [image(String uid, String picid)](#image-java.lang.String-java.lang.String-) | Bild‑Stream abrufen. |
| [imageUrl(String baseURL, String picid, String uid)](#imageUrl-java.lang.String-java.lang.String-java.lang.String-) | Liefert die Bild‑URL. |
| [lazyLoadingJson(String sheetName, String uid)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Liefert den JSON‑String des angegebenen Tabellenblatts in der Datei aus dem Cache mittels der angegebenen eindeutigen ID. |
| [lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)](#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-) | Schreibt den JSON‑String des angegebenen Tabellenblatts in der Datei aus dem Cache mittels der angegebenen eindeutigen ID in den Stream. |
| [load(String uid, String filename)](#load-java.lang.String-java.lang.String-) | Liefert den JSON‑String der Datei aus dem Cache anhand der angegebenen eindeutigen ID, setzt den Ausgabedateinamen im JSON. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [ole(String uid, String sheetname, int oleid, String label)](#ole-java.lang.String-java.lang.String-int-java.lang.String-) | Liefert die Byte‑Array‑Daten des eingebetteten OLE‑Objekts. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridjs.GridWorkbookSettings-) | Stellt die Arbeitsmappeneinstellungen dar. |
| [toString()](#toString--) |  |
| [translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)](#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-) | Übersetzt alle Zeichenkettenwerte im Arbeitsblatt in die Zielsprache. |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Führt die Update‑Operation aus. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsService(GridJsOptions options) {#GridJsService-com.aspose.gridjs.GridJsOptions-}
```
public GridJsService(GridJsOptions options)
```


Der Standardkonstruktor für GridJsService

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | [GridJsOptions](../../com.aspose.gridjs/gridjsoptions) |  |

### addImage(String p, String uid, InputStream filestream) {#addImage-java.lang.String-java.lang.String-java.io.InputStream-}
```
public String addImage(String p, String uid, InputStream filestream)
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
public String addImageByURL(String p, String uid, InputStream filestream, String imageurl)
```


Wendet die Operation zum Hinzufügen eines Bildes aus einer lokalen Datei an.

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
public boolean checkInCacheForCollaborative(String uid)
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
public void clearAllJsonCache()
```


Löscht alle JSON-Cache‑Einträge (Speicher und Festplatte).

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public void clearJsonCacheForUid(String uid)
```


Löscht alle JSON-Cache-Einträge, die zur angegebenen eindeutigen ID gehören. Rufen Sie dies auf, nachdem Sie die Quelldatei außerhalb des normalen Ablaufs geändert haben, damit die nächste Anforderung das JSON neu generiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |

### copyImage(String p, String uid) {#copyImage-java.lang.String-java.lang.String-}
```
public String copyImage(String p, String uid)
```


Führt die Kopier‑Bild‑Operation aus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| p | java.lang.String | Der JSON‑String‑Parameter |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |

**Returns:**
java.lang.String - Das JSON‑String‑Ergebnis
### destroy() {#destroy--}
```
public void destroy()
```


Diese Methode ist nur für Java vorgesehen, sie implementiert die destroy‑Methode in DisposableBean, die von Spring automatisch aufgerufen wird, wenn die Anfrage abgeschlossen ist; tatsächlich ruft sie die Dispose‑Methode auf.

### detailFileJsonWithUid(String filePath, String uid) {#detailFileJsonWithUid-java.lang.String-java.lang.String-}
```
public StringBuilder detailFileJsonWithUid(String filePath, String uid)
```


Liefert den JSON‑String für die Datei anhand der angegebenen eindeutigen ID.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Der vollständige Dateipfad |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |

**Returns:**
java.lang.StringBuilder
### detailStreamJson(OutputStream stream, String filePath) {#detailStreamJson-java.io.OutputStream-java.lang.String-}
```
public void detailStreamJson(OutputStream stream, String filePath)
```


Schreibt den JSON‑String für die Datei in den Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Stream, der geschrieben wird |
| filePath | java.lang.String | Der vollständige Dateipfad |

### detailStreamJsonWithUid(OutputStream stream, String filePath, String uid) {#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)
```


Schreibt den JSON‑String für die Datei in den Stream anhand der angegebenen eindeutigen ID.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Stream, der geschrieben wird |
| filePath | java.lang.String | Der vollständige Dateipfad |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |

### dispose() {#dispose--}
```
public void dispose()
```


Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind.

### download(String p, String uid, String filename) {#download-java.lang.String-java.lang.String-java.lang.String-}
```
public String download(String p, String uid, String filename)
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
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
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


Datei‑Stream abrufen

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileid | java.lang.String | die Datei-ID |

**Returns:**
java.io.InputStream - Der Stream der Datei
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Stellt die Arbeitsmappeneinstellungen dar.

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
public String imageUrl(String baseURL, String picid, String uid)
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
public StringBuilder lazyLoadingJson(String sheetName, String uid)
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
public void lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)
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
public String load(String uid, String filename)
```


Liefert den JSON‑String der Datei aus dem Cache anhand der angegebenen eindeutigen ID, setzt den Ausgabedateinamen im JSON.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |
| Dateiname | java.lang.String | Gibt den Dateinamen im JSON an. Wenn er auf null gesetzt wird, ist der Standarddateiname: book1. |

**Returns:**
java.lang.String - Der JSON-String
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
### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridjs.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Stellt die Arbeitsmappeneinstellungen dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
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


Übersetzt alle Zeichenkettenwerte im Arbeitsblatt in die Zielsprache.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |
| sheetName | java.lang.String | Der Blattname |
| translator | [ITextTranslator](../../com.aspose.gridjs/itexttranslator) | Der Übersetzer, der die translate-Funktion implementiert |
| targetLanguage | java.lang.String | Die Zielsprache |

**Returns:**
java.lang.String -
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public String updateCell(String p, String uid)
```


Führt die Update‑Operation aus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| p | java.lang.String | Der JSON-Format-String der Aktualisierungsoperation. |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

