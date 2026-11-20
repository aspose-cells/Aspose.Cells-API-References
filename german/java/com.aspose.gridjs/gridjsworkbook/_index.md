---
title: "GridJsWorkbook"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Haupt‑Einstiegsklasse für GridJs dar"
type: docs
url: /de/java/com.aspose.gridjs/gridjsworkbook/
---

**Inheritance:**
java.lang.Object
```
public class GridJsWorkbook
```

Stellt die Haupt‑Einstiegsklasse für GridJs dar
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [GridJsWorkbook()](#GridJsWorkbook--) | Erstellt eine neue Instanz von GridJsWorkbook. |
## Felder

| Feld | Beschreibung |
| --- | --- |
| [CacheImp](#CacheImp) | Benutzerdefinierte Implementierung für den Cache-Speicher. Wenn Sie den Cache in Stream-Form speichern möchten, müssen Sie ihn setzen und implementieren. |
| [CalculateEngine](#CalculateEngine) | Benutzerdefinierte Implementierung für die Berechnungs-Engine, wenn Sie benutzerdefinierte Berechnungen durchführen möchten, müssen Sie sie festlegen und implementieren. |
| [PICTURE_TYPE](#PICTURE-TYPE) | Konstanter Wert für den Bildtyp |
| [UpdateMonitor](#UpdateMonitor) | Liest/Setzt den Update-Monitor, um die Aktualisierungsoperation zu verfolgen |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [burnRedactionFile(String excelFilePath, String uid)](#burnRedactionFile-java.lang.String-java.lang.String-) | Führt (wendet) alle Redaktionsoperationen in der Arbeitsmappe aus, indem Redaktionsformen und deren Zielformen entfernt oder der Inhalt des Zielzellenbereichs gelöscht wird. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Überprüfen Sie, ob die Workbook-Instanz im Speicher-Cache ist. Diese Methode wird nur für den Collaborative‑Modus angewendet. |
| [clearAllJsonCache()](#clearAllJsonCache--) | \\u5a13\\u5474\\u6ace\\u93b5\\u20ac\\u93c8? |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | \\u93cd\\u89c4\\u5d41 uid \\u5a13\\u5474\\u6ace JSON \\u7f02\\u64b3\\u74e8\\u951b\\u5822\\u6564\\u6d5c? |
| [copyImageOrShape(String uid, String p)](#copyImageOrShape-java.lang.String-java.lang.String-) | Kopiert Bild oder Form. |
| [dispose()](#dispose--) | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [errorJson(String msg)](#errorJson-java.lang.String-) | Liest die Fehlermeldungszeichenkette im JSON-Format. |
| [exportToJson()](#exportToJson--) | Liest JSON-String aus dem Speicher, der Standarddateiname im JSON ist: book1. |
| [exportToJson(String filename)](#exportToJson-java.lang.String-) | Liest JSON-String aus dem Speicher, setzt den Ausgabedateinamen im JSON. |
| [exportToJsonStringBuilder(String filename)](#exportToJsonStringBuilder-java.lang.String-) | Liest JSON-String aus dem Speicher, setzt den Ausgabedateinamen im JSON. |
| [exportToJsonStringBuilder(String filename, String uid)](#exportToJsonStringBuilder-java.lang.String-java.lang.String-) |  |
| [getCacheDirectory()](#getCacheDirectory--) | Ermittelt das Cache-Verzeichnis zum Speichern von Tabellenkalkulationsdateien. |
| [getClass()](#getClass--) |  |
| [getGridLoadFormat(String extension)](#getGridLoadFormat-java.lang.String-) | Liest das Ladeformat anhand der Dateierweiterung. |
| [getImageStream(String uid, String picid, String cachedir)](#getImageStream-java.lang.String-java.lang.String-java.lang.String-) | Bild‑Stream abrufen. |
| [getImageUrl(String uid, String picid, String delimiter)](#getImageUrl-java.lang.String-java.lang.String-java.lang.String-) | Liefert die Bild‑URL. |
| [getJsonByUid(String uid, String filename)](#getJsonByUid-java.lang.String-java.lang.String-) | Liefert den JSON‑String der Datei aus dem Cache anhand der angegebenen eindeutigen ID, setzt den Ausgabedateinamen im JSON. |
| [getOle(String uid, String sheetname, int oleid, String label)](#getOle-java.lang.String-java.lang.String-int-java.lang.String-) | Liefert die Byte‑Array‑Daten des eingebetteten OLE‑Objekts. |
| [getSettings()](#getSettings--) | Stellt die Arbeitsmappeneinstellungen dar. |
| [getSheetJsonWithCache(String uid, String sheetName, String fileName)](#getSheetJsonWithCache-java.lang.String-java.lang.String-java.lang.String-) | \\u947e\\u5cf0\\u5f47\\u93b8\\u56e7\\u757e sheet \\u9428? |
| [getUidForFile(String fileName)](#getUidForFile-java.lang.String-) | Erzeugt eine neue eindeutige ID für den Dateicache anhand des angegebenen Dateinamens. |
| [getWorkbookJsonWithCache(String uid, String fileName)](#getWorkbookJsonWithCache-java.lang.String-java.lang.String-) | \\u947e\\u5cf0\\u5f47\\u93c1\\u7fe0\\u91dc\\u5bb8\\u30e4\\u7d94\\u7ee8\\u8de8\\u6b91 JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b? |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream filestream, int format)](#importExcelFile-java.io.InputStream-int-) | Importiert die Excel-Datei aus dem Dateistream mit Ladeformat. |
| [importExcelFile(InputStream filestream, int format, String password)](#importExcelFile-java.io.InputStream-int-java.lang.String-) | Importiert die Excel-Datei aus dem Dateistream mit Ladeformat und Öffnungspasswort. |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | Importiert die Excel-Datei vom Dateipfad. |
| [importExcelFile(String uid, InputStream filestream, int format)](#importExcelFile-java.lang.String-java.io.InputStream-int-) | Importiert die Excel-Datei aus dem Dateistream. |
| [importExcelFile(String uid, InputStream filestream, int format, String password)](#importExcelFile-java.lang.String-java.io.InputStream-int-java.lang.String-) | Importiert die Excel-Datei aus dem Dateistream mit Ladeformat und Öffnungspasswort. |
| [importExcelFile(String uid, String fileName)](#importExcelFile-java.lang.String-java.lang.String-) | Importiert die Excel-Datei vom Dateipfad. |
| [importExcelFile(String uid, String fileName, String password)](#importExcelFile-java.lang.String-java.lang.String-java.lang.String-) | Importiert die Excel-Datei vom Dateipfad und Öffnungspasswort. |
| [importExcelFileFromJson(String json)](#importExcelFileFromJson-java.lang.String-) | Importiert die Excel-Datei aus einem JSON-Format-String. |
| [insertImage(String uid, String p, InputStream s, String imageUrl)](#insertImage-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Fügt ein Bild im Arbeitsblatt aus einem Dateistream oder der URL ein (entweder der Dateistream oder die URL muss bereitgestellt werden) oder fügt eine Form ein, wenn p.type einer von AutoShapeType ist. |
| [jsonToStream(OutputStream stream, String filename)](#jsonToStream-java.io.OutputStream-java.lang.String-) | Erzeugt JSON aus dem im Speicher befindlichen Workbook und schreibt es in den angegebenen Stream. |
| [jsonToStream(OutputStream stream, String filename, String uid)](#jsonToStream-java.io.OutputStream-java.lang.String-java.lang.String-) |  |
| [jsonToStreamByUid(OutputStream stream, String uid, String filename)](#jsonToStreamByUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Ruft den JSON-String der Datei aus dem Cache mit der angegebenen eindeutigen ID ab, setzt den Ausgabedateinamen im JSON und schreibt ihn in den Stream. |
| [lazyLoadingJson(String uid, String sheetName)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Liefert den JSON‑String des angegebenen Tabellenblatts in der Datei aus dem Cache mittels der angegebenen eindeutigen ID. |
| [lazyLoadingStream(OutputStream stream, String uid, String sheetName)](#lazyLoadingStream-java.io.OutputStream-java.lang.String-java.lang.String-) | Ruft den JSON-String des angegebenen Arbeitsblatts in der Datei aus dem Cache mit der angegebenen eindeutigen ID ab und schreibt ihn in den Stream. |
| [mergeExcelFileFromJson(String uid, String json)](#mergeExcelFileFromJson-java.lang.String-java.lang.String-) | Wendet ein Batch-Update auf die Speicherdaten an. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr)](#redactFile-java.lang.String-java.lang.String-java.lang.String---) | Führt eine Redaktion einer Excel-Datei basierend auf einem Array von JSON-Operationen durch. |
| [saveToCacheWithFileName(String uid, String filename, String password)](#saveToCacheWithFileName-java.lang.String-java.lang.String-java.lang.String-) | Speichert die Speicherdaten in die Cache-Datei mit dem angegebenen Dateinamen und setzt zudem das Öffnungspasswort, das Speicherformat basiert auf der Dateierweiterung des Dateinamens. |
| [saveToExcelFile(OutputStream stream)](#saveToExcelFile-java.io.OutputStream-) | Speichert die Speicherdaten in den Stream, basierend auf dem ursprünglichen Dateiformat. |
| [saveToExcelFile(String path)](#saveToExcelFile-java.lang.String-) | Speichert die Speicherdaten im Dateipfad, falls die Datei eine Erweiterung hat, basiert das Speicherformat auf der Dateierweiterung. |
| [saveToHtml(OutputStream stream)](#saveToHtml-java.io.OutputStream-) | Speichert die Speicherdaten in den Stream, das Speicherformat ist HTML. |
| [saveToHtml(String path)](#saveToHtml-java.lang.String-) | Speichert die Speicherdaten im Dateipfad, das Speicherformat ist HTML. |
| [saveToPdf(OutputStream stream)](#saveToPdf-java.io.OutputStream-) | Speichert die Speicherdaten in den Stream, das Speicherformat ist PDF. |
| [saveToPdf(String path)](#saveToPdf-java.lang.String-) | Speichert die Speicherdaten im Dateipfad, das Speicherformat ist PDF. |
| [saveToXlsx(OutputStream stream)](#saveToXlsx-java.io.OutputStream-) | Speichert die Speicherdaten in den Stream, das Speicherformat ist XLSX. |
| [saveToXlsx(String path)](#saveToXlsx-java.lang.String-) | Speichert die Speicherdaten im Dateipfad, das Speicherformat ist XLSX. |
| [setCacheDirectory(String value)](#setCacheDirectory-java.lang.String-) | Legt das Cache‑Verzeichnis zum Speichern von Tabellenkalkulationsdateien fest. |
| [setImageUrlBase(String baseImageURL)](#setImageUrlBase-java.lang.String-) | Setzt die Basis-Bild‑Abruf‑URL vom Controller. |
| [setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds)](#setInterruptMonitorForLoad-com.aspose.gridjs.GridInterruptMonitor-int-) | Setzt InterruptMonitor für Ladevorgänge. |
| [setInterruptMonitorForSave(GridInterruptMonitor monitor)](#setInterruptMonitorForSave-com.aspose.gridjs.GridInterruptMonitor-) | Setzt InterruptMonitor für Speicher‑Vorgänge. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridjs.GridWorkbookSettings-) | Stellt die Arbeitsmappeneinstellungen dar. |
| [setTransParentView(String excelFilePath, String uid, boolean isTransparent)](#setTransParentView-java.lang.String-java.lang.String-boolean-) | Setzt die Transparenz der Redaktionsformen im Workbook. |
| [toString()](#toString--) |  |
| [translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)](#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-) | Übersetzt alle Zeichenkettenwerte im Arbeitsblatt in die Zielsprache. |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Führt die Update‑Operation aus. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsWorkbook() {#GridJsWorkbook--}
```
public GridJsWorkbook()
```


Erstellt eine neue Instanz von GridJsWorkbook.

### CacheImp {#CacheImp}
```
public static GridCacheForStream CacheImp
```


Benutzerdefinierte Implementierung für den Cache-Speicher. Wenn Sie den Cache in Stream-Form speichern möchten, müssen Sie ihn setzen und implementieren.

### CalculateEngine {#CalculateEngine}
```
public static GridAbstractCalculationEngine CalculateEngine
```


Benutzerdefinierte Implementierung für die Berechnungs-Engine, wenn Sie benutzerdefinierte Berechnungen durchführen möchten, müssen Sie sie festlegen und implementieren.

### PICTURE_TYPE {#PICTURE-TYPE}
```
public static final String PICTURE_TYPE
```


Konstanter Wert für den Bildtyp

### UpdateMonitor {#UpdateMonitor}
```
public static GridUpdateMonitor UpdateMonitor
```


Liest/Setzt den Update-Monitor, um die Aktualisierungsoperation zu verfolgen

### burnRedactionFile(String excelFilePath, String uid) {#burnRedactionFile-java.lang.String-java.lang.String-}
```
public void burnRedactionFile(String excelFilePath, String uid)
```


Führt (wendet) alle Redaktionsoperationen in der Arbeitsmappe aus, indem Redaktionsformen und deren Zielformen entfernt oder der Inhalt des Zielzellenbereichs gelöscht wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| excelFilePath | java.lang.String | Der Dateipfad der Excel-Datei. |
| uid | java.lang.String | Der eindeutige Bezeichner für das Workbook. Wenn null oder leer, wird eine neue UID basierend auf dem Dateipfad generiert. |

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


\\u5a13\\u5474\\u6ace\\u93b5\\u20ac\\u93c8?JSON \\u7f02\\u64b3\\u74e8

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public void clearJsonCacheForUid(String uid)
```


\\u93cd\\u89c4\\u5d41 uid \\u5a13\\u5474\\u6ace JSON \\u7f02\\u64b3\\u74e8\\u951b\\u5822\\u6564\\u6d5c?UpdateCell \\u7edb\\u590a\\u5f67\\u93c8?uid \\u9428\\u52eb\\u6e80\\u93c5\\ue224\\u7d1a

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |

### copyImageOrShape(String uid, String p) {#copyImageOrShape-java.lang.String-java.lang.String-}
```
public String copyImageOrShape(String uid, String p)
```


Kopiert Bild oder Form.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |
| p | java.lang.String | Der JSON-String für die Operation, die den Zellort angibt, enthält den Arbeitsblattnamen, die obere linke Zeile und die obere linke Spalte für das Bild oder die Form\\u951b\\u5b94tc {name:'sheet1',ri:1,ci:1,srcid:2,srcname:'sheet2',isshape:true} |

**Returns:**
java.lang.String - Der JSON-String des neu kopierten Bildes
### dispose() {#dispose--}
```
public void dispose()
```


Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind.

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
### errorJson(String msg) {#errorJson-java.lang.String-}
```
public String errorJson(String msg)
```


Liest die Fehlermeldungszeichenkette im JSON-Format.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| msg | java.lang.String | Die Fehlermeldung. |

**Returns:**
java.lang.String - Der JSON-String.
### exportToJson() {#exportToJson--}
```
public String exportToJson()
```


Liest JSON-String aus dem Speicher, der Standarddateiname im JSON ist: book1.

**Returns:**
java.lang.String - Der JSON-String.
### exportToJson(String filename) {#exportToJson-java.lang.String-}
```
public String exportToJson(String filename)
```


Liest JSON-String aus dem Speicher, setzt den Ausgabedateinamen im JSON.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Dateiname | java.lang.String | Gibt den Dateinamen im JSON an. Wenn null gesetzt, ist der Standarddateiname: book1.. |

**Returns:**
java.lang.String - Der JSON-String.
### exportToJsonStringBuilder(String filename) {#exportToJsonStringBuilder-java.lang.String-}
```
public StringBuilder exportToJsonStringBuilder(String filename)
```


Liest JSON-String aus dem Speicher, setzt den Ausgabedateinamen im JSON.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Dateiname | java.lang.String | Gibt den Dateinamen im JSON an. Wenn null gesetzt, ist der Standarddateiname: book1.. |

**Returns:**
java.lang.StringBuilder - Der JSON-StringBuilder.
### exportToJsonStringBuilder(String filename, String uid) {#exportToJsonStringBuilder-java.lang.String-java.lang.String-}
```
public StringBuilder exportToJsonStringBuilder(String filename, String uid)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Dateiname | java.lang.String |  |
| uid | java.lang.String |  |

**Returns:**
java.lang.StringBuilder
### getCacheDirectory() {#getCacheDirectory--}
```
public String getCacheDirectory()
```


Ermittelt das Cache-Verzeichnis zum Speichern der Tabellenkalkulationsdatei. Wenn dies nicht gesetzt ist, verwenden wir die statische Eigenschaft von [Config.getFileCacheDirectory()](../../com.aspose.gridjs/config\#getFileCacheDirectory--) oder [CacheImp](../../com.aspose.gridjs/gridjsworkbook\#CacheImp).

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


Liest das Ladeformat anhand der Dateierweiterung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| extension | java.lang.String | Die Dateierweiterung, beginnt normalerweise mit '.'. |

**Returns:**
int - [GridLoadFormat](../../com.aspose.gridjs/gridloadformat).
### getImageStream(String uid, String picid, String cachedir) {#getImageStream-java.lang.String-java.lang.String-java.lang.String-}
```
public static InputStream getImageStream(String uid, String picid, String cachedir)
```


Bild‑Stream abrufen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |
| picid | java.lang.String | Die Bild-ID. |
| cachedir | java.lang.String |  |

**Returns:**
java.io.InputStream - Der Bild-Stream
### getImageUrl(String uid, String picid, String delimiter) {#getImageUrl-java.lang.String-java.lang.String-java.lang.String-}
```
public static String getImageUrl(String uid, String picid, String delimiter)
```


Liefert die Bild‑URL.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |
| picid | java.lang.String | Die Bild-ID. |
| delimiter | java.lang.String | Das Trennzeichen der Zeichenkette. |

**Returns:**
java.lang.String -
### getJsonByUid(String uid, String filename) {#getJsonByUid-java.lang.String-java.lang.String-}
```
public StringBuilder getJsonByUid(String uid, String filename)
```


Liefert den JSON‑String der Datei aus dem Cache anhand der angegebenen eindeutigen ID, setzt den Ausgabedateinamen im JSON.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |
| Dateiname | java.lang.String | Gibt den Dateinamen im JSON an. Wenn er auf null gesetzt wird, ist der Standarddateiname: book1. |

**Returns:**
java.lang.StringBuilder - Der JSON-String-StringBuilder
### getOle(String uid, String sheetname, int oleid, String label) {#getOle-java.lang.String-java.lang.String-int-java.lang.String-}
```
public byte[] getOle(String uid, String sheetname, int oleid, String label)
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
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Stellt die Arbeitsmappeneinstellungen dar.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings)
### getSheetJsonWithCache(String uid, String sheetName, String fileName) {#getSheetJsonWithCache-java.lang.String-java.lang.String-java.lang.String-}
```
public String getSheetJsonWithCache(String uid, String sheetName, String fileName)
```


\\u947e\\u5cf0\\u5f47\\u93b8\\u56e7\\u757e sheet \\u9428?JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b?\*

**Parameters:**
| Parameter | Typ | Beschreibung |
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


Erzeugt eine neue eindeutige ID für den Dateicache anhand des angegebenen Dateinamens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der Dateiname. |

**Returns:**
java.lang.String -
### getWorkbookJsonWithCache(String uid, String fileName) {#getWorkbookJsonWithCache-java.lang.String-java.lang.String-}
```
public String getWorkbookJsonWithCache(String uid, String fileName)
```


\\u947e\\u5cf0\\u5f47\\u93c1\\u7fe0\\u91dc\\u5bb8\\u30e4\\u7d94\\u7ee8\\u8de8\\u6b91 JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b?\*

**Parameters:**
| Parameter | Typ | Beschreibung |
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


Importiert die Excel-Datei aus dem Dateistream mit Ladeformat.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filestream | java.io.InputStream | Der Stream der Excel-Datei. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). Das Ladeformat der Excel-Datei. |

### importExcelFile(InputStream filestream, int format, String password) {#importExcelFile-java.io.InputStream-int-java.lang.String-}
```
public void importExcelFile(InputStream filestream, int format, String password)
```


Importiert die Excel-Datei aus dem Dateistream mit Ladeformat und Öffnungspasswort.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filestream | java.io.InputStream | Der Stream der Excel-Datei. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). Das Ladeformat der Excel-Datei. |
| Passwort | java.lang.String | Das Öffnungspasswort der Excel-Datei. Der Wert kann null sein, wenn kein Passwort gesetzt ist. |

### importExcelFile(String fileName) {#importExcelFile-java.lang.String-}
```
public void importExcelFile(String fileName)
```


Importiert die Excel-Datei vom Dateipfad.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der vollständige Pfad der Datei. |

### importExcelFile(String uid, InputStream filestream, int format) {#importExcelFile-java.lang.String-java.io.InputStream-int-}
```
public void importExcelFile(String uid, InputStream filestream, int format)
```


Importiert die Excel-Datei aus dem Dateistream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache, wenn null gesetzt, wird sie automatisch erzeugt. |
| filestream | java.io.InputStream | Der Stream der Excel-Datei. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). Das Ladeformat der Excel-Datei. |

### importExcelFile(String uid, InputStream filestream, int format, String password) {#importExcelFile-java.lang.String-java.io.InputStream-int-java.lang.String-}
```
public void importExcelFile(String uid, InputStream filestream, int format, String password)
```


Importiert die Excel-Datei aus dem Dateistream mit Ladeformat und Öffnungspasswort.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache, wenn null gesetzt, wird sie automatisch erzeugt. |
| filestream | java.io.InputStream | Der Stream der Excel-Datei. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). Das Ladeformat der Excel-Datei. |
| Passwort | java.lang.String | Das Öffnungspasswort der Excel-Datei. Der Wert kann null sein, wenn kein Passwort gesetzt ist. |

### importExcelFile(String uid, String fileName) {#importExcelFile-java.lang.String-java.lang.String-}
```
public void importExcelFile(String uid, String fileName)
```


Importiert die Excel-Datei vom Dateipfad.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache, wenn null gesetzt, wird sie automatisch erzeugt. |
| fileName | java.lang.String | Der vollständige Pfad der Datei. |

### importExcelFile(String uid, String fileName, String password) {#importExcelFile-java.lang.String-java.lang.String-java.lang.String-}
```
public void importExcelFile(String uid, String fileName, String password)
```


Importiert die Excel-Datei vom Dateipfad und Öffnungspasswort.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache, wenn null gesetzt, wird sie automatisch erzeugt. |
| fileName | java.lang.String | Der vollständige Pfad der Datei. |
| Passwort | java.lang.String | Das Öffnungspasswort der Excel-Datei. Der Wert kann null sein, wenn kein Passwort gesetzt ist. |

### importExcelFileFromJson(String json) {#importExcelFileFromJson-java.lang.String-}
```
public void importExcelFileFromJson(String json)
```


Importiert die Excel-Datei aus einem JSON-Format-String.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| JSON | java.lang.String | Der JSON-Format-String. |

### insertImage(String uid, String p, InputStream s, String imageUrl) {#insertImage-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-}
```
public String insertImage(String uid, String p, InputStream s, String imageUrl)
```


Fügt ein Bild im Arbeitsblatt aus einem Dateistream oder der URL ein (entweder der Dateistream oder die URL muss bereitgestellt werden) oder fügt eine Form ein, wenn p.type einer von AutoShapeType ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache |
| p | java.lang.String | Der JSON-Format-String für die Operation, die den Zellort, den Arbeitsblattnamen, die obere linke Zeile und die obere linke Spalte für das Bild\\u951b\\u5b94tc \{name:'sheet1',ri:1,ci:1\} |
| s | java.io.InputStream | Der Dateistream der Bilddatei |
| imageUrl | java.lang.String | Die URL der Bilddatei |

**Returns:**
java.lang.String - Der JSON-Format-String des eingefügten Bildes
### jsonToStream(OutputStream stream, String filename) {#jsonToStream-java.io.OutputStream-java.lang.String-}
```
public void jsonToStream(OutputStream stream, String filename)
```


Generieren Sie JSON aus dem im Speicher befindlichen Workbook und schreiben Sie es in den angegebenen Stream. Optional wird das erzeugte JSON zwischengespeichert, um spätere Abrufe zu beschleunigen. Wesentliche Unterschiede zu JsonToStreamByUid: - Diese Methode verwendet den aktuellen im Speicher befindlichen Workbook-Zustand (wb-Feld) - JsonToStreamByUid lädt das Workbook aus .cells-Cache-Dateien auf der Festplatte neu - Verwenden Sie diese Methode, wenn Sie den aktuellen Workbook-Zustand nach Änderungen exportieren möchten - Verwenden Sie JsonToStreamByUid, wenn Sie JSON aus einem zuvor zwischengespeicherten Dateizustand neu generieren müssen Caching‑Verhalten (wenn uid angegeben ist): - Prüft den JSON-Cache vor der Erzeugung (L1‑Speicher + L2‑Disk) - Bei einem Cache‑Fehltritt wird JSON aus dem im Speicher befindlichen Workbook generiert - Speichert das erzeugte JSON im Cache für zukünftige Anfragen

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Ausgabestream, in den JSON-Daten geschrieben werden |
| Dateiname | java.lang.String | Gibt den Dateinamen im JSON an. Wenn er auf null gesetzt wird, ist der Standarddateiname: book1. |

### jsonToStream(OutputStream stream, String filename, String uid) {#jsonToStream-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void jsonToStream(OutputStream stream, String filename, String uid)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream |  |
| Dateiname | java.lang.String |  |
| uid | java.lang.String |  |

### jsonToStreamByUid(OutputStream stream, String uid, String filename) {#jsonToStreamByUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public boolean jsonToStreamByUid(OutputStream stream, String uid, String filename)
```


Ruft den JSON-String der Datei aus dem Cache mit der angegebenen eindeutigen ID ab, setzt den Ausgabedateinamen im JSON und schreibt ihn in den Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Stream, der geschrieben wird |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |
| Dateiname | java.lang.String | Gibt den Dateinamen im JSON an. Wenn er auf null gesetzt wird, ist der Standarddateiname: book1. |

**Returns:**
boolean
### lazyLoadingJson(String uid, String sheetName) {#lazyLoadingJson-java.lang.String-java.lang.String-}
```
public StringBuilder lazyLoadingJson(String uid, String sheetName)
```


Liefert den JSON‑String des angegebenen Tabellenblatts in der Datei aus dem Cache mittels der angegebenen eindeutigen ID.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |
| sheetName | java.lang.String | der Blattname. |

**Returns:**
java.lang.StringBuilder - Der JSON-String-StringBuilder
### lazyLoadingStream(OutputStream stream, String uid, String sheetName) {#lazyLoadingStream-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void lazyLoadingStream(OutputStream stream, String uid, String sheetName)
```


Ruft den JSON-String des angegebenen Arbeitsblatts in der Datei aus dem Cache mit der angegebenen eindeutigen ID ab und schreibt ihn in den Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Stream, der geschrieben wird |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |
| sheetName | java.lang.String | der Blattname. |

### mergeExcelFileFromJson(String uid, String json) {#mergeExcelFileFromJson-java.lang.String-java.lang.String-}
```
public void mergeExcelFileFromJson(String uid, String json)
```


Wendet ein Batch-Update auf die Speicherdaten an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |
| JSON | java.lang.String | Der Aktualisierungs‑JSON-Format-String. |

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


Führt eine Redaktion einer Excel-Datei basierend auf einem Array von JSON-Operationen durch.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| excelFilePath | java.lang.String | Der Dateipfad der zu redigierenden Excel-Datei. |
| uid | java.lang.String | Der eindeutige Bezeichner für das Workbook. Wenn null oder leer, wird eine neue UID basierend auf dem Dateipfad generiert. |
| arrayOfRedactionOpr | java.lang.String[] | Ein Array von JSON-Strings, die die anzuwendenden Redaktionsoperationen darstellen. |

### saveToCacheWithFileName(String uid, String filename, String password) {#saveToCacheWithFileName-java.lang.String-java.lang.String-java.lang.String-}
```
public void saveToCacheWithFileName(String uid, String filename, String password)
```


Speichert die Speicherdaten in die Cache-Datei mit dem angegebenen Dateinamen und setzt zudem das Öffnungspasswort, das Speicherformat basiert auf der Dateierweiterung des Dateinamens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |
| Dateiname | java.lang.String | Der Dateiname zum Speichern. |
| Passwort | java.lang.String | Das Öffnungspasswort der Excel-Datei. Der Wert kann null sein, wenn kein Passwort festgelegt ist. |

### saveToExcelFile(OutputStream stream) {#saveToExcelFile-java.io.OutputStream-}
```
public void saveToExcelFile(OutputStream stream)
```


Speichert die Speicherdaten in den Stream, basierend auf dem ursprünglichen Dateiformat.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Stream zum Speichern. |

### saveToExcelFile(String path) {#saveToExcelFile-java.lang.String-}
```
public void saveToExcelFile(String path)
```


Speichert die Speicherdaten im Dateipfad, falls die Datei eine Erweiterung hat, basiert das Speicherformat auf der Dateierweiterung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | java.lang.String | Der Dateipfad zum Speichern. |

### saveToHtml(OutputStream stream) {#saveToHtml-java.io.OutputStream-}
```
public void saveToHtml(OutputStream stream)
```


Speichert die Speicherdaten in den Stream, das Speicherformat ist HTML.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Stream zum Speichern. |

### saveToHtml(String path) {#saveToHtml-java.lang.String-}
```
public void saveToHtml(String path)
```


Speichert die Speicherdaten im Dateipfad, das Speicherformat ist HTML.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | java.lang.String | Der Dateipfad zum Speichern. |

### saveToPdf(OutputStream stream) {#saveToPdf-java.io.OutputStream-}
```
public void saveToPdf(OutputStream stream)
```


Speichert die Speicherdaten in den Stream, das Speicherformat ist PDF.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Stream zum Speichern. |

### saveToPdf(String path) {#saveToPdf-java.lang.String-}
```
public void saveToPdf(String path)
```


Speichert die Speicherdaten im Dateipfad, das Speicherformat ist PDF.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | java.lang.String | Der Dateipfad zum Speichern. |

### saveToXlsx(OutputStream stream) {#saveToXlsx-java.io.OutputStream-}
```
public void saveToXlsx(OutputStream stream)
```


Speichert die Speicherdaten in den Stream, das Speicherformat ist XLSX.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Stream zum Speichern. |

### saveToXlsx(String path) {#saveToXlsx-java.lang.String-}
```
public void saveToXlsx(String path)
```


Speichert die Speicherdaten im Dateipfad, das Speicherformat ist XLSX.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | java.lang.String | Der Dateipfad zum Speichern. |

### setCacheDirectory(String value) {#setCacheDirectory-java.lang.String-}
```
public void setCacheDirectory(String value)
```


Legt das Cache-Verzeichnis für die Speicherung von Tabellenkalkulationsdateien fest. Wenn dies nicht gesetzt ist, verwenden wir die statische Eigenschaft von [Config.getFileCacheDirectory()](../../com.aspose.gridjs/config\#getFileCacheDirectory--) oder [CacheImp](../../com.aspose.gridjs/gridjsworkbook\#CacheImp).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setImageUrlBase(String baseImageURL) {#setImageUrlBase-java.lang.String-}
```
public static void setImageUrlBase(String baseImageURL)
```


Setzt die Basis-Bild‑Abruf‑URL vom Controller.

**Remarks**

Wenn CacheImp null ist, muss dies gesetzt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| baseImageURL | java.lang.String | Die Basis-URL für die Bild‑Abruf‑Aktion. |

### setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds) {#setInterruptMonitorForLoad-com.aspose.gridjs.GridInterruptMonitor-int-}
```
public void setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds)
```


Setzt InterruptMonitor für Ladevorgänge.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| monitor | [GridInterruptMonitor](../../com.aspose.gridjs/gridinterruptmonitor) | Die InterruptMonitor-Instanz. |
| calculateTimeoutMilliseconds | int | Der Timeout in Millisekunden für das Laden der Datei. |

### setInterruptMonitorForSave(GridInterruptMonitor monitor) {#setInterruptMonitorForSave-com.aspose.gridjs.GridInterruptMonitor-}
```
public void setInterruptMonitorForSave(GridInterruptMonitor monitor)
```


Setzt InterruptMonitor für Speicher‑Vorgänge.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| monitor | [GridInterruptMonitor](../../com.aspose.gridjs/gridinterruptmonitor) | Die InterruptMonitor-Instanz. |

### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridjs.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Stellt die Arbeitsmappeneinstellungen dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings) |  |

### setTransParentView(String excelFilePath, String uid, boolean isTransparent) {#setTransParentView-java.lang.String-java.lang.String-boolean-}
```
public void setTransParentView(String excelFilePath, String uid, boolean isTransparent)
```


Setzt die Transparenz der Redaktionsformen im Workbook.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| excelFilePath | java.lang.String | Der Dateipfad der Excel-Datei. |
| uid | java.lang.String | Der eindeutige Bezeichner für das Workbook. Wenn null oder leer, wird eine neue UID basierend auf dem Dateipfad generiert. |
| isTransparent | boolean | Wenn true, setzt die Transparenz auf 0,89 (halbtransparent); wenn false, setzt die Transparenz auf 1 (vollständig undurchsichtig/unsichtbar). |

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
java.lang.String – Die JSON‑Formatzeichenkette des Aktualisierungsergebnisses.
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

