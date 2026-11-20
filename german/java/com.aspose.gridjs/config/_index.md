---
title: "Konfiguration"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt alle statischen Einstellungen für GridJs dar"
type: docs
url: /de/java/com.aspose.gridjs/config/
---

**Inheritance:**
java.lang.Object
```
public class Config
```

Stellt alle statischen Einstellungen für GridJs dar
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Config()](#Config--) |  |
## Felder

| Feld | Beschreibung |
| --- | --- |
| [RedactionUseClientGenerateId](#RedactionUseClientGenerateId) | Gibt an, ob in redaktionsbezogenen Vorgängen die vom Client generierte ID anstelle der tatsächlichen Shape-ID verwendet wird |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitColumnsOnLoad()](#getAutoFitColumnsOnLoad--) | Gibt an, ob die Spaltenbreiten beim Laden der Datei automatisch angepasst werden sollen. |
| [getAutoFitRowsHeightOnLoad()](#getAutoFitRowsHeightOnLoad--) | Gibt an, ob die Zeilenhöhen beim Laden der Datei automatisch angepasst werden sollen. |
| [getAutoOptimizeForLargeCells()](#getAutoOptimizeForLargeCells--) | Ermittelt, ob die Ladeleistung für Arbeitsblätter mit großen Zellen automatisch optimiert werden soll. |
| [getBaseRouteName()](#getBaseRouteName--) | Liefert den Basisroutennamen für die GridJs‑Controller‑URL. Der Standardwert ist "/GridJs2". |
| [getClass()](#getClass--) |  |
| [getEmptySheetMaxCol()](#getEmptySheetMaxCol--) | Ermittelt die standardmäßige maximale Spaltenanzahl für ein leeres Arbeitsblatt. |
| [getEmptySheetMaxRow()](#getEmptySheetMaxRow--) | Ermittelt die standardmäßige maximale Zeilenanzahl für ein leeres Arbeitsblatt. |
| [getEnableChartClientRendering()](#getEnableChartClientRendering--) | Ermittelt, ob die clientseitige Diagrammdarstellung aktiviert werden soll. |
| [getFileCacheDirectory()](#getFileCacheDirectory--) | Ermittelt das Cache-Verzeichnis zum Speichern von Tabellenkalkulationsdateien. |
| [getIgnoreEmptyContent()](#getIgnoreEmptyContent--) | Ermittelt, ob der maximale Bereich angezeigt werden soll, der Daten, Formatierungen, zusammengeführte Zellen und Shapes umfasst. |
| [getIslimitShapeOrImage()](#getIslimitShapeOrImage--) | Ermittelt, ob die Gesamtzahl der angezeigten Shapes/Bilder in einem Arbeitsblatt begrenzt werden soll. Wenn auf true gesetzt, begrenzt GridJs die Gesamtzahl der angezeigten Shapes oder Bilder in einem Arbeitsblatt auf MaxShapeOrImageCount, der Standardwert ist true. |
| [getJsonCache()](#getJsonCache--) | Ermittelt die JSON-Cache-Konfigurationsoptionen. |
| [getLazyLoading()](#getLazyLoading--) | Ermittelt, ob nur das aktive Arbeitsblatt geladen werden soll, der Standardwert ist false. |
| [getMaxPdfSaveSeconds()](#getMaxPdfSaveSeconds--) | Ermittelt die maximal zulässige Zeitüberschreitung in Sekunden beim Speichern als PDF. |
| [getMaxShapeOrImageCount()](#getMaxShapeOrImageCount--) | Ermittelt die Gesamtzahl der angezeigten Shapes oder Bilder im aktiven Blatt, wirksam wenn IslimitShapeOrImage=true. |
| [getMaxShapeOrImageWidthOrHeight()](#getMaxShapeOrImageWidthOrHeight--) | Ermittelt die maximale Breite oder Höhe für ein Shape oder ein Bild. GridJs ignoriert Shapes oder Bilder, deren Breite oder Höhe größer ist, wirksam wenn IslimitShapeOrImage=true. |
| [getMaxTotalShapeOrImageCount()](#getMaxTotalShapeOrImageCount--) | Ermittelt die Gesamtzahl der angezeigten Shapes oder Bilder in der Arbeitsmappe, wirksam wenn IslimitShapeOrImage=true. |
| [getMessageTopic()](#getMessageTopic--) | Liefert die Websocket‑Ziele, die mit "/topic" beginnen. Der Standard ist "/topic/opr". Wird nur im kollaborativen Modus verwendet. |
| [getPictureCacheDirectory()](#getPictureCacheDirectory--) | Liefert das Cache‑Verzeichnis für Bilder. |
| [getSameImageDetecting()](#getSameImageDetecting--) | Liefert, ob geprüft werden soll, ob Bilder dieselbe Quelle haben; der Standardwert ist true. |
| [getSaveHtmlAsZip()](#getSaveHtmlAsZip--) | Liefert, ob HTML‑Dateien als ZIP‑Archiv gespeichert werden sollen, der Standardwert ist false. |
| [getShowChartSheet()](#getShowChartSheet--) | Liefert, ob das Diagramm‑Arbeitsblatt angezeigt werden soll. |
| [getSkipInvisibleShapes()](#getSkipInvisibleShapes--) | Liefert, ob Formen, die für die UI unsichtbar sind, übersprungen werden sollen, der Standardwert ist true. |
| [getUsePrintArea()](#getUsePrintArea--) | Liefert, ob PageSetup.PrintArea für den UI‑Anzeigebereich verwendet werden soll, wenn das Arbeitsblatt eine PageSetup‑Einstellung für PrintArea hat. |
| [hashCode()](#hashCode--) |  |
| [isCollaborative()](#isCollaborative--) | Liefert, ob kollaboratives Bearbeiten unterstützt wird, der Standardwert ist false. |
| [isWasm()](#isWasm--) | Liefert, ob GridJs innerhalb eines Browser‑WebAssembly‑Hosts anstelle eines Serverprozesses ausgeführt wird. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFitColumnsOnLoad(boolean value)](#setAutoFitColumnsOnLoad-boolean-) | Gibt an, ob die Spaltenbreiten beim Laden der Datei automatisch angepasst werden sollen. |
| [setAutoFitRowsHeightOnLoad(boolean value)](#setAutoFitRowsHeightOnLoad-boolean-) | Gibt an, ob die Zeilenhöhen beim Laden der Datei automatisch angepasst werden sollen. |
| [setAutoOptimizeForLargeCells(boolean value)](#setAutoOptimizeForLargeCells-boolean-) | Legt fest, ob die Ladeleistung für Arbeitsblätter mit großen Zellen automatisch optimiert werden soll. |
| [setBaseRouteName(String value)](#setBaseRouteName-java.lang.String-) | Setzt den Basisroutennamen für die GridJs‑Controller‑URL. Der Standardwert ist "/GridJs2". |
| [setCollaborative(boolean value)](#setCollaborative-boolean-) | Legt fest, ob kollaboratives Bearbeiten unterstützt wird, der Standardwert ist false. |
| [setEmptySheetMaxCol(int value)](#setEmptySheetMaxCol-int-) | Legt die standardmäßige maximale Spaltenzahl für ein leeres Arbeitsblatt fest. |
| [setEmptySheetMaxRow(int value)](#setEmptySheetMaxRow-int-) | Legt die standardmäßige maximale Zeilenzahl für ein leeres Arbeitsblatt fest. |
| [setEnableChartClientRendering(boolean value)](#setEnableChartClientRendering-boolean-) | Legt fest, ob die clientseitige Diagrammdarstellung aktiviert werden soll. |
| [setFileCacheDirectory(String value)](#setFileCacheDirectory-java.lang.String-) | Legt das Cache‑Verzeichnis zum Speichern von Tabellenkalkulationsdateien fest. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Legt den Schriftarten-Ordner fest |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Setzt die Schriftordner |
| [setIgnoreEmptyContent(boolean value)](#setIgnoreEmptyContent-boolean-) | Legt fest, ob der maximale Bereich angezeigt werden soll, der Daten, Formatierungen, zusammengeführte Zellen und Formen umfasst. |
| [setIslimitShapeOrImage(boolean value)](#setIslimitShapeOrImage-boolean-) | Legt fest, ob die Gesamtzahl der angezeigten Formen/Bilder in einem Arbeitsblatt begrenzt werden soll; ist der Wert true, begrenzt GridJs die Gesamtzahl der angezeigten Formen oder Bilder in einem Arbeitsblatt auf MaxShapeOrImageCount. Der Standardwert ist true. |
| [setJsonCache(JsonCacheOptions value)](#setJsonCache-com.aspose.gridjs.JsonCacheOptions-) | Legt Optionen für die JSON‑Cache‑Konfiguration fest. |
| [setLazyLoading(boolean value)](#setLazyLoading-boolean-) | Legt fest, ob nur das aktive Arbeitsblatt geladen werden soll, der Standardwert ist false. |
| [setMaxPdfSaveSeconds(int value)](#setMaxPdfSaveSeconds-int-) | Legt die maximal zulässige Zeitüberschreitung in Sekunden beim Speichern als PDF fest. |
| [setMaxShapeOrImageCount(int value)](#setMaxShapeOrImageCount-int-) | Legt die Gesamtzahl der angezeigten Formen oder Bilder im aktiven Blatt fest; wirksam, wenn IslimitShapeOrImage=true. |
| [setMaxShapeOrImageWidthOrHeight(int value)](#setMaxShapeOrImageWidthOrHeight-int-) | Legt die maximale Breite oder Höhe für eine Form oder ein Bild fest; GridJs ignoriert Formen oder Bilder, deren Breite oder Höhe größer ist, wirksam, wenn IslimitShapeOrImage=true. |
| [setMaxTotalShapeOrImageCount(int value)](#setMaxTotalShapeOrImageCount-int-) | Legt die Gesamtzahl der angezeigten Formen oder Bilder in der Arbeitsmappe fest; wirksam, wenn IslimitShapeOrImage=true. |
| [setMessageTopic(String value)](#setMessageTopic-java.lang.String-) | Legt die Websocket‑Ziele fest, die mit "\/topic" beginnen. Der Standard ist "\/topic/opr". Wird nur im kollaborativen Modus verwendet. |
| [setPictureCacheDirectory(String value)](#setPictureCacheDirectory-java.lang.String-) | Legt das Cache-Verzeichnis für Bilder fest. |
| [setSameImageDetecting(boolean value)](#setSameImageDetecting-boolean-) | Legt fest, ob geprüft wird, ob Bilder dieselbe Quelle haben, der Standardwert ist true. |
| [setSaveHtmlAsZip(boolean value)](#setSaveHtmlAsZip-boolean-) | Legt fest, ob HTML-Dateien als ZIP-Archiv gespeichert werden, der Standardwert ist false. |
| [setShowChartSheet(boolean value)](#setShowChartSheet-boolean-) | Legt fest, ob das Diagramm-Arbeitsblatt angezeigt wird. |
| [setSkipInvisibleShapes(boolean value)](#setSkipInvisibleShapes-boolean-) | Legt fest, ob Formen, die für die UI unsichtbar sind, übersprungen werden, der Standardwert ist true. |
| [setUsePrintArea(boolean value)](#setUsePrintArea-boolean-) | Legt fest, ob PageSetup.PrintArea für den UI-Anzeigebereich verwendet wird, wenn das Arbeitsblatt eine PageSetup-Einstellung für PrintArea hat. |
| [setWasm(boolean value)](#setWasm-boolean-) | Legt fest, ob GridJs innerhalb eines Browser‑WebAssembly‑Hosts anstelle eines Serverprozesses ausgeführt wird. |
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


Gibt an, ob in redaktionsbezogenen Vorgängen die vom Client generierte ID anstelle der tatsächlichen Shape-ID verwendet wird

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
### getAutoFitColumnsOnLoad() {#getAutoFitColumnsOnLoad--}
```
public static boolean getAutoFitColumnsOnLoad()
```


Gibt an, ob die Spaltenbreiten beim Laden der Datei automatisch angepasst werden sollen. Der Standardwert ist `false`. Hinweis: Das Setzen auf `true` führt nach dem Laden zu einer automatischen Anpassung aller Spalten, was die Leistung merklich beeinträchtigen kann.

**Returns:**
boolean
### getAutoFitRowsHeightOnLoad() {#getAutoFitRowsHeightOnLoad--}
```
public static boolean getAutoFitRowsHeightOnLoad()
```


Gibt an, ob die Zeilenhöhen beim Laden der Datei automatisch angepasst werden sollen. Der Standardwert ist `false`. Hinweis: Das Setzen auf `true` führt nach dem Laden zu einer automatischen Anpassung aller Zeilen, was die Leistung merklich beeinträchtigen kann.

**Returns:**
boolean
### getAutoOptimizeForLargeCells() {#getAutoOptimizeForLargeCells--}
```
public static boolean getAutoOptimizeForLargeCells()
```


Ermittelt, ob die Ladeleistung für Arbeitsblätter mit großen Zellen automatisch optimiert wird. Es werden einige Stile/Grenzen ignoriert, um die Ladezeit zu verkürzen. Der Standardwert ist true.

**Returns:**
boolean
### getBaseRouteName() {#getBaseRouteName--}
```
public static String getBaseRouteName()
```


Liefert den Basisroutennamen für die GridJs‑Controller‑URL. Der Standardwert ist "/GridJs2".

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


Ermittelt die standardmäßige maximale Spaltenanzahl für ein leeres Arbeitsblatt. Der Standardwert ist 15.

**Returns:**
int
### getEmptySheetMaxRow() {#getEmptySheetMaxRow--}
```
public static int getEmptySheetMaxRow()
```


Ermittelt die standardmäßige maximale Zeilenanzahl für ein leeres Arbeitsblatt. Der Standardwert ist 12.

**Returns:**
int
### getEnableChartClientRendering() {#getEnableChartClientRendering--}
```
public static boolean getEnableChartClientRendering()
```


Liefert, ob die clientseitige Diagrammdarstellung aktiviert ist. Wenn auf false gesetzt, fällt GridJs auf ausschließlich serverseitig erzeugte Diagrammbilder/-formen zurück. Der Standardwert ist true.

**Returns:**
boolean
### getFileCacheDirectory() {#getFileCacheDirectory--}
```
public static String getFileCacheDirectory()
```


Ermittelt das Cache‑Verzeichnis zum Speichern von Tabellenkalkulationsdateien. Wir müssen es vor der Verwendung von GridJs auf einen bestimmten Pfad setzen.

**Returns:**
java.lang.String
### getIgnoreEmptyContent() {#getIgnoreEmptyContent--}
```
public static boolean getIgnoreEmptyContent()
```


Ermittelt, ob der maximale Bereich angezeigt wird, der Daten, Stil, zusammengeführte Zellen und Formen enthält. Wenn die letzte Zeile oder Spalte Zellen ohne Wert und Formel, aber mit benutzerdefiniertem Stil enthält, wird diese Zeile/Spalte nicht angezeigt, wenn dieser Wert true ist\u9286?\* Der Standardwert ist true.

**Returns:**
boolean
### getIslimitShapeOrImage() {#getIslimitShapeOrImage--}
```
public static boolean getIslimitShapeOrImage()
```


Ermittelt, ob die Gesamtzahl der angezeigten Shapes/Bilder in einem Arbeitsblatt begrenzt werden soll. Wenn auf true gesetzt, begrenzt GridJs die Gesamtzahl der angezeigten Shapes oder Bilder in einem Arbeitsblatt auf MaxShapeOrImageCount, der Standardwert ist true.

**Returns:**
boolean
### getJsonCache() {#getJsonCache--}
```
public static JsonCacheOptions getJsonCache()
```


Ermittelt die JSON‑Cache‑Konfigurationsoptionen. Steuert das Verhalten des Speicher‑ (L1) und Festplatten‑ (L2) Caches für das erzeugte Arbeitsbuch‑JSON.

**Returns:**
[JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions)
### getLazyLoading() {#getLazyLoading--}
```
public static boolean getLazyLoading()
```


Ermittelt, ob nur das aktive Arbeitsblatt geladen werden soll, der Standardwert ist false.

**Returns:**
boolean
### getMaxPdfSaveSeconds() {#getMaxPdfSaveSeconds--}
```
public static int getMaxPdfSaveSeconds()
```


Ermittelt die maximal zulässige Zeitüberschreitung in Sekunden beim Speichern als PDF. Der Standardwert ist 10.

**Returns:**
int
### getMaxShapeOrImageCount() {#getMaxShapeOrImageCount--}
```
public static int getMaxShapeOrImageCount()
```


Ermittelt die Gesamtzahl der angezeigten Formen oder Bilder im aktiven Blatt, wirksam wenn IslimitShapeOrImage=true. Der Standardwert ist 100.

**Returns:**
int
### getMaxShapeOrImageWidthOrHeight() {#getMaxShapeOrImageWidthOrHeight--}
```
public static int getMaxShapeOrImageWidthOrHeight()
```


Ermittelt die maximale Breite oder Höhe für eine Form oder ein Bild. GridJs ignoriert Formen oder Bilder, deren Breite oder Höhe größer ist, wirksam wenn IslimitShapeOrImage=true. Der Standardwert ist 10000.

**Returns:**
int
### getMaxTotalShapeOrImageCount() {#getMaxTotalShapeOrImageCount--}
```
public static int getMaxTotalShapeOrImageCount()
```


Ermittelt die Gesamtzahl der angezeigten Formen oder Bilder im Arbeitsbuch, wirksam wenn IslimitShapeOrImage=true. Der Standardwert ist 300.

**Returns:**
int
### getMessageTopic() {#getMessageTopic--}
```
public static String getMessageTopic()
```


Liefert die Websocket‑Ziele, die mit "/topic" beginnen. Der Standard ist "/topic/opr". Wird nur im kollaborativen Modus verwendet.

**Returns:**
java.lang.String
### getPictureCacheDirectory() {#getPictureCacheDirectory--}
```
public static String getPictureCacheDirectory()
```


Ermittelt das Cache‑Verzeichnis für Bilder. (Wirksam, wenn GridJsWorkbook.CacheImp null ist) Der Standardpfad ist "\\_piccache" im FileCacheDirectory.

**Returns:**
java.lang.String
### getSameImageDetecting() {#getSameImageDetecting--}
```
public static boolean getSameImageDetecting()
```


Liefert, ob geprüft werden soll, ob Bilder dieselbe Quelle haben; der Standardwert ist true.

**Returns:**
boolean
### getSaveHtmlAsZip() {#getSaveHtmlAsZip--}
```
public static boolean getSaveHtmlAsZip()
```


Liefert, ob HTML‑Dateien als ZIP‑Archiv gespeichert werden sollen, der Standardwert ist false.

**Returns:**
boolean
### getShowChartSheet() {#getShowChartSheet--}
```
public static boolean getShowChartSheet()
```


Ermittelt, ob das Diagramm‑Arbeitsblatt angezeigt wird. Der Standardwert ist false.

**Returns:**
boolean
### getSkipInvisibleShapes() {#getSkipInvisibleShapes--}
```
public static boolean getSkipInvisibleShapes()
```


Liefert, ob Formen, die für die UI unsichtbar sind, übersprungen werden sollen, der Standardwert ist true.

**Returns:**
boolean
### getUsePrintArea() {#getUsePrintArea--}
```
public static boolean getUsePrintArea()
```


Ermittelt, ob PageSetup.PrintArea für den UI-Anzeigebereich verwendet wird, wenn das Arbeitsblatt eine PageSetup‑Einstellung für PrintArea hat. Der Standardwert ist false.

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


Liefert, ob kollaboratives Bearbeiten unterstützt wird, der Standardwert ist false.

**Returns:**
boolean
### isWasm() {#isWasm--}
```
public static boolean isWasm()
```


Liefert, ob GridJs in einem Browser‑WebAssembly‑Host anstelle eines Serverprozesses ausgeführt wird. Wenn true, wird kein FileCacheDirectory / Festplatte / Interrupt‑Thread‑Pfad verwendet und der Dateicache muss von GridJsOptions.CacheImp stammen. GridJsOptions.IsWasm setzt dies, wenn der GridJs‑Dienst erstellt wird, sodass eine Aspose.Cells.GridJs.dll beide Hosts bedient. Der Standardwert ist false.

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


Gibt an, ob die Spaltenbreiten beim Laden der Datei automatisch angepasst werden sollen. Der Standardwert ist `false`. Hinweis: Das Setzen auf `true` führt nach dem Laden zu einer automatischen Anpassung aller Spalten, was die Leistung merklich beeinträchtigen kann.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAutoFitRowsHeightOnLoad(boolean value) {#setAutoFitRowsHeightOnLoad-boolean-}
```
public static void setAutoFitRowsHeightOnLoad(boolean value)
```


Gibt an, ob die Zeilenhöhen beim Laden der Datei automatisch angepasst werden sollen. Der Standardwert ist `false`. Hinweis: Das Setzen auf `true` führt nach dem Laden zu einer automatischen Anpassung aller Zeilen, was die Leistung merklich beeinträchtigen kann.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAutoOptimizeForLargeCells(boolean value) {#setAutoOptimizeForLargeCells-boolean-}
```
public static void setAutoOptimizeForLargeCells(boolean value)
```


Legt fest, ob die Ladeleistung für Arbeitsblätter mit großen Zellen automatisch optimiert wird. Es werden einige Stile/Grenzen ignoriert, um die Ladezeit zu verkürzen. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setBaseRouteName(String value) {#setBaseRouteName-java.lang.String-}
```
public static void setBaseRouteName(String value)
```


Setzt den Basisroutennamen für die GridJs‑Controller‑URL. Der Standardwert ist "/GridJs2".

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCollaborative(boolean value) {#setCollaborative-boolean-}
```
public static void setCollaborative(boolean value)
```


Legt fest, ob kollaboratives Bearbeiten unterstützt wird, der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEmptySheetMaxCol(int value) {#setEmptySheetMaxCol-int-}
```
public static void setEmptySheetMaxCol(int value)
```


Legt die maximale Standardspaltenzahl für ein leeres Arbeitsblatt fest. Der Standardwert ist 15.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setEmptySheetMaxRow(int value) {#setEmptySheetMaxRow-int-}
```
public static void setEmptySheetMaxRow(int value)
```


Legt die maximale Standardzeilenzahl für ein leeres Arbeitsblatt fest. Der Standardwert ist 12.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setEnableChartClientRendering(boolean value) {#setEnableChartClientRendering-boolean-}
```
public static void setEnableChartClientRendering(boolean value)
```


Setzt, ob die clientseitige Diagrammdarstellung aktiviert ist. Wenn auf false gesetzt, fällt GridJs auf ausschließlich serverseitig erzeugte Diagrammbilder/-formen zurück. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFileCacheDirectory(String value) {#setFileCacheDirectory-java.lang.String-}
```
public static void setFileCacheDirectory(String value)
```


Legt das Cache‑Verzeichnis zum Speichern von Tabellenkalkulationsdateien fest. Wir müssen es vor der Verwendung von GridJs auf einen bestimmten Pfad setzen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```


Legt den Schriftarten-Ordner fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontFolder | java.lang.String | Der Ordner, der TrueType-Schriftarten enthält. |
| rekursiv | boolean | Bestimmt, ob Unterordner gescannt werden sollen oder nicht. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


Setzt die Schriftordner

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Die Ordner, die TrueType-Schriften enthalten. |
| rekursiv | boolean | Bestimmt, ob Unterordner gescannt werden sollen oder nicht. |

### setIgnoreEmptyContent(boolean value) {#setIgnoreEmptyContent-boolean-}
```
public static void setIgnoreEmptyContent(boolean value)
```


Legt fest, ob der maximale Bereich, der Daten, Stil, zusammengeführte Zellen und Formen enthält, angezeigt wird. Wenn die letzte Zeile oder Spalte Zellen ohne Wert und Formel, aber mit benutzerdefiniertem Stil enthält, wird diese Zeile/Spalte nicht angezeigt, wenn dieser Wert true ist\\u9286?\* Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setIslimitShapeOrImage(boolean value) {#setIslimitShapeOrImage-boolean-}
```
public static void setIslimitShapeOrImage(boolean value)
```


Legt fest, ob die Gesamtzahl der angezeigten Formen/Bilder in einem Arbeitsblatt begrenzt werden soll; ist der Wert true, begrenzt GridJs die Gesamtzahl der angezeigten Formen oder Bilder in einem Arbeitsblatt auf MaxShapeOrImageCount. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setJsonCache(JsonCacheOptions value) {#setJsonCache-com.aspose.gridjs.JsonCacheOptions-}
```
public static void setJsonCache(JsonCacheOptions value)
```


Legt die JSON‑Cache‑Konfigurationsoptionen fest. Steuert sowohl das Speicher‑ (L1) als auch das Festplatten‑ (L2) Cache‑Verhalten für das erzeugte Arbeitsbuch‑JSON.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions) |  |

### setLazyLoading(boolean value) {#setLazyLoading-boolean-}
```
public static void setLazyLoading(boolean value)
```


Legt fest, ob nur das aktive Arbeitsblatt geladen werden soll, der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setMaxPdfSaveSeconds(int value) {#setMaxPdfSaveSeconds-int-}
```
public static void setMaxPdfSaveSeconds(int value)
```


Legt die maximalen Zeitüberschreitungssekunden beim Speichern als PDF fest. Der Standardwert ist 10.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMaxShapeOrImageCount(int value) {#setMaxShapeOrImageCount-int-}
```
public static void setMaxShapeOrImageCount(int value)
```


Legt die Gesamtanzahl der angezeigten Formen oder Bilder im aktiven Blatt fest, wirksam wenn IslimitShapeOrImage=true. Der Standardwert ist 100.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMaxShapeOrImageWidthOrHeight(int value) {#setMaxShapeOrImageWidthOrHeight-int-}
```
public static void setMaxShapeOrImageWidthOrHeight(int value)
```


Legt die maximale Breite oder Höhe für eine Form oder ein Bild fest; GridJs ignoriert Formen oder Bilder, deren Breite oder Höhe größer ist, wirksam wenn IslimitShapeOrImage=true. Der Standardwert ist 10000.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMaxTotalShapeOrImageCount(int value) {#setMaxTotalShapeOrImageCount-int-}
```
public static void setMaxTotalShapeOrImageCount(int value)
```


Legt die Gesamtanzahl der angezeigten Formen oder Bilder im Arbeitsbuch fest, wirksam wenn IslimitShapeOrImage=true. Der Standardwert ist 300.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMessageTopic(String value) {#setMessageTopic-java.lang.String-}
```
public static void setMessageTopic(String value)
```


Legt die Websocket‑Ziele fest, die mit "\/topic" beginnen. Der Standard ist "\/topic/opr". Wird nur im kollaborativen Modus verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setPictureCacheDirectory(String value) {#setPictureCacheDirectory-java.lang.String-}
```
public static void setPictureCacheDirectory(String value)
```


Legt das Cache‑Verzeichnis für Bilder fest (dies wirkt, wenn GridJsWorkbook.CacheImp null ist). Der Standardpfad ist "\\_piccache" im FileCacheDirectory.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setSameImageDetecting(boolean value) {#setSameImageDetecting-boolean-}
```
public static void setSameImageDetecting(boolean value)
```


Legt fest, ob geprüft wird, ob Bilder dieselbe Quelle haben, der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSaveHtmlAsZip(boolean value) {#setSaveHtmlAsZip-boolean-}
```
public static void setSaveHtmlAsZip(boolean value)
```


Legt fest, ob HTML-Dateien als ZIP-Archiv gespeichert werden, der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowChartSheet(boolean value) {#setShowChartSheet-boolean-}
```
public static void setShowChartSheet(boolean value)
```


Legt fest, ob das Diagramm‑Arbeitsblatt angezeigt wird. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSkipInvisibleShapes(boolean value) {#setSkipInvisibleShapes-boolean-}
```
public static void setSkipInvisibleShapes(boolean value)
```


Legt fest, ob Formen, die für die UI unsichtbar sind, übersprungen werden, der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setUsePrintArea(boolean value) {#setUsePrintArea-boolean-}
```
public static void setUsePrintArea(boolean value)
```


Legt fest, ob PageSetup.PrintArea für den UI‑Anzeigebereich verwendet wird, wenn das Arbeitsblatt eine PageSetup‑Einstellung für PrintArea hat. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setWasm(boolean value) {#setWasm-boolean-}
```
public static void setWasm(boolean value)
```


Setzt, ob GridJs in einem Browser‑WebAssembly‑Host anstelle eines Serverprozesses ausgeführt wird. Wenn true, wird kein FileCacheDirectory / Festplatte / Interrupt‑Thread‑Pfad verwendet und der Dateicache muss von GridJsOptions.CacheImp stammen. GridJsOptions.IsWasm setzt dies, wenn der GridJs‑Dienst erstellt wird, sodass eine Aspose.Cells.GridJs.dll beide Hosts bedient. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

