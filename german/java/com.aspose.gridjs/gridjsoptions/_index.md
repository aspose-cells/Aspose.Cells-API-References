---
title: "GridJsOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt alle Ladeoptionen für GridJs dar"
type: docs
url: /de/java/com.aspose.gridjs/gridjsoptions/
---

**Inheritance:**
java.lang.Object
```
public class GridJsOptions
```

Stellt alle Ladeoptionen für GridJs dar
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [GridJsOptions()](#GridJsOptions--) |  |
## Felder

| Feld | Beschreibung |
| --- | --- |
| [CacheImp](#CacheImp) | Benutzerdefinierte Implementierung für den Cache-Speicher. Wenn Sie den Cache in Stream-Form speichern möchten, müssen Sie ihn setzen und implementieren. |
| [RedactionUseClientGenerateId](#RedactionUseClientGenerateId) | Gibt an, ob in redaktionsbezogenen Vorgängen die vom Client generierte ID anstelle der tatsächlichen Shape-ID verwendet wird |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitColumnsOnLoad()](#getAutoFitColumnsOnLoad--) | Gibt an, ob die Spaltenbreite beim Laden der Datei automatisch angepasst werden soll, der Standardwert ist false. |
| [getAutoFitRowsHeightOnLoad()](#getAutoFitRowsHeightOnLoad--) | Gibt an, ob die Zeilenhöhe beim Laden der Datei automatisch angepasst werden soll, der Standardwert ist false. |
| [getAutoOptimizeForLargeCells()](#getAutoOptimizeForLargeCells--) | Ermittelt, ob die Ladeleistung für Arbeitsblätter mit großen Zellen automatisch optimiert werden soll. |
| [getBaseRouteName()](#getBaseRouteName--) | Ermittelt den Basisnamen der Routen-URL für den GridJs-Controller, der Standard ist GridJs2. |
| [getClass()](#getClass--) |  |
| [getEmptySheetMaxCol()](#getEmptySheetMaxCol--) | Ermittelt die standardmäßige maximale Spaltenanzahl für ein leeres Arbeitsblatt. |
| [getEmptySheetMaxRow()](#getEmptySheetMaxRow--) | Ermittelt die standardmäßige maximale Zeilenanzahl für ein leeres Arbeitsblatt. |
| [getEnableChartClientRendering()](#getEnableChartClientRendering--) | Ermittelt, ob die clientseitige Diagrammdarstellung aktiviert werden soll. |
| [getFileCacheDirectory()](#getFileCacheDirectory--) | Ermittelt das Cache-Verzeichnis zum Speichern von Tabellenkalkulationsdateien. |
| [getFontFolders()](#getFontFolders--) | Ermittelt die Schriftartenordner für Schriften in gerenderten Bildern/Shapes |
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
| [setAutoFitColumnsOnLoad(boolean value)](#setAutoFitColumnsOnLoad-boolean-) | Gibt an, ob die Spaltenbreite beim Laden der Datei automatisch angepasst werden soll, der Standardwert ist false. |
| [setAutoFitRowsHeightOnLoad(boolean value)](#setAutoFitRowsHeightOnLoad-boolean-) | Gibt an, ob die Zeilenhöhe beim Laden der Datei automatisch angepasst werden soll, der Standardwert ist false. |
| [setAutoOptimizeForLargeCells(boolean value)](#setAutoOptimizeForLargeCells-boolean-) | Legt fest, ob die Ladeleistung für Arbeitsblätter mit großen Zellen automatisch optimiert werden soll. |
| [setBaseRouteName(String value)](#setBaseRouteName-java.lang.String-) | Legt den Basisnamen der Routen‑URL für den GridJs‑Controller fest. Der Standard ist GridJs2. |
| [setCollaborative(boolean value)](#setCollaborative-boolean-) | Legt fest, ob kollaboratives Bearbeiten unterstützt wird, der Standardwert ist false. |
| [setEmptySheetMaxCol(int value)](#setEmptySheetMaxCol-int-) | Legt die standardmäßige maximale Spaltenzahl für ein leeres Arbeitsblatt fest. |
| [setEmptySheetMaxRow(int value)](#setEmptySheetMaxRow-int-) | Legt die standardmäßige maximale Zeilenzahl für ein leeres Arbeitsblatt fest. |
| [setEnableChartClientRendering(boolean value)](#setEnableChartClientRendering-boolean-) | Legt fest, ob die clientseitige Diagrammdarstellung aktiviert werden soll. |
| [setFileCacheDirectory(String value)](#setFileCacheDirectory-java.lang.String-) | Legt das Cache‑Verzeichnis zum Speichern von Tabellenkalkulationsdateien fest. |
| [setFontFolders(String[] value)](#setFontFolders-java.lang.String---) | Legt die Schriftordner für Schriften in gerenderten Bildern/Formen fest. |
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
### GridJsOptions() {#GridJsOptions--}
```
public GridJsOptions()
```


### CacheImp {#CacheImp}
```
public GridCacheForStream CacheImp
```


Benutzerdefinierte Implementierung für den Cache‑Speicher. Wenn Sie den Cache als Stream speichern möchten, müssen Sie ihn setzen und implementieren. Ein WebAssembly‑Host (IsWasm = true) muss ihn setzen, da für den Standard‑Dateicache kein lokaler Datenträger vorhanden ist.

### RedactionUseClientGenerateId {#RedactionUseClientGenerateId}
```
public boolean RedactionUseClientGenerateId
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
public boolean getAutoFitColumnsOnLoad()
```


Gibt an, ob die Spaltenbreite beim Laden der Datei automatisch angepasst werden soll, der Standardwert ist false.

**Returns:**
boolean
### getAutoFitRowsHeightOnLoad() {#getAutoFitRowsHeightOnLoad--}
```
public boolean getAutoFitRowsHeightOnLoad()
```


Gibt an, ob die Zeilenhöhe beim Laden der Datei automatisch angepasst werden soll, der Standardwert ist false.

**Returns:**
boolean
### getAutoOptimizeForLargeCells() {#getAutoOptimizeForLargeCells--}
```
public boolean getAutoOptimizeForLargeCells()
```


Ermittelt, ob die Ladeleistung für Arbeitsblätter mit großen Zellen automatisch optimiert wird. Es werden einige Stile/Grenzen ignoriert, um die Ladezeit zu verkürzen. Der Standardwert ist true.

**Returns:**
boolean
### getBaseRouteName() {#getBaseRouteName--}
```
public String getBaseRouteName()
```


Ermittelt den Basisnamen der Routen-URL für den GridJs-Controller, der Standard ist GridJs2.

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
public int getEmptySheetMaxCol()
```


Ermittelt die standardmäßige maximale Spaltenanzahl für ein leeres Arbeitsblatt. Der Standardwert ist 15.

**Returns:**
int
### getEmptySheetMaxRow() {#getEmptySheetMaxRow--}
```
public int getEmptySheetMaxRow()
```


Ermittelt die standardmäßige maximale Zeilenanzahl für ein leeres Arbeitsblatt. Der Standardwert ist 12.

**Returns:**
int
### getEnableChartClientRendering() {#getEnableChartClientRendering--}
```
public boolean getEnableChartClientRendering()
```


Ermittelt, ob die clientseitige Diagramm‑Renderung aktiviert ist. Wenn auf false gesetzt, gibt GridJs nur Diagrammbilder/-formen aus und erfordert keine clientseitige Diagramm‑Renderung. Der Standardwert ist true.

**Returns:**
boolean
### getFileCacheDirectory() {#getFileCacheDirectory--}
```
public String getFileCacheDirectory()
```


Ermittelt das Cache‑Verzeichnis zum Speichern von Tabellenkalkulationsdateien. Wir müssen es vor der Verwendung von GridJs auf einen bestimmten Pfad setzen.

**Returns:**
java.lang.String
### getFontFolders() {#getFontFolders--}
```
public String[] getFontFolders()
```


Ermittelt die Schriftartenordner für Schriften in gerenderten Bildern/Shapes

**Returns:**
java.lang.String[]
### getIgnoreEmptyContent() {#getIgnoreEmptyContent--}
```
public boolean getIgnoreEmptyContent()
```


Ermittelt, ob der maximale Bereich angezeigt wird, der Daten, Stil, zusammengeführte Zellen und Formen enthält. Wenn die letzte Zeile oder Spalte Zellen ohne Wert und Formel, aber mit benutzerdefiniertem Stil enthält, wird diese Zeile/Spalte nicht angezeigt, wenn dieser Wert true ist\u9286?\* Der Standardwert ist true.

**Returns:**
boolean
### getIslimitShapeOrImage() {#getIslimitShapeOrImage--}
```
public boolean getIslimitShapeOrImage()
```


Ermittelt, ob die Gesamtzahl der angezeigten Shapes/Bilder in einem Arbeitsblatt begrenzt werden soll. Wenn auf true gesetzt, begrenzt GridJs die Gesamtzahl der angezeigten Shapes oder Bilder in einem Arbeitsblatt auf MaxShapeOrImageCount, der Standardwert ist true.

**Returns:**
boolean
### getJsonCache() {#getJsonCache--}
```
public JsonCacheOptions getJsonCache()
```


Ermittelt die JSON‑Cache‑Konfigurationsoptionen. Steuert das Verhalten des Speicher‑ (L1) und Festplatten‑ (L2) Caches für das erzeugte Arbeitsbuch‑JSON.

**Returns:**
[JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions)
### getLazyLoading() {#getLazyLoading--}
```
public boolean getLazyLoading()
```


Ermittelt, ob nur das aktive Arbeitsblatt geladen werden soll, der Standardwert ist false.

**Returns:**
boolean
### getMaxPdfSaveSeconds() {#getMaxPdfSaveSeconds--}
```
public int getMaxPdfSaveSeconds()
```


Ermittelt die maximal zulässige Zeitüberschreitung in Sekunden beim Speichern als PDF. Der Standardwert ist 10.

**Returns:**
int
### getMaxShapeOrImageCount() {#getMaxShapeOrImageCount--}
```
public int getMaxShapeOrImageCount()
```


Ermittelt die Gesamtzahl der angezeigten Formen oder Bilder im aktiven Blatt, wirksam wenn IslimitShapeOrImage=true. Der Standardwert ist 100.

**Returns:**
int
### getMaxShapeOrImageWidthOrHeight() {#getMaxShapeOrImageWidthOrHeight--}
```
public int getMaxShapeOrImageWidthOrHeight()
```


Ermittelt die maximale Breite oder Höhe für eine Form oder ein Bild. GridJs ignoriert Formen oder Bilder, deren Breite oder Höhe größer ist, wirksam wenn IslimitShapeOrImage=true. Der Standardwert ist 10000.

**Returns:**
int
### getMaxTotalShapeOrImageCount() {#getMaxTotalShapeOrImageCount--}
```
public int getMaxTotalShapeOrImageCount()
```


Ermittelt die Gesamtzahl der angezeigten Formen oder Bilder im Arbeitsbuch, wirksam wenn IslimitShapeOrImage=true. Der Standardwert ist 300.

**Returns:**
int
### getMessageTopic() {#getMessageTopic--}
```
public String getMessageTopic()
```


Liefert die Websocket‑Ziele, die mit "/topic" beginnen. Der Standard ist "/topic/opr". Wird nur im kollaborativen Modus verwendet.

**Returns:**
java.lang.String
### getPictureCacheDirectory() {#getPictureCacheDirectory--}
```
public String getPictureCacheDirectory()
```


Ermittelt das Cache‑Verzeichnis für Bilder. (Wirksam, wenn GridJsWorkbook.CacheImp null ist) Der Standardpfad ist "\\_piccache" im FileCacheDirectory.

**Returns:**
java.lang.String
### getSameImageDetecting() {#getSameImageDetecting--}
```
public boolean getSameImageDetecting()
```


Liefert, ob geprüft werden soll, ob Bilder dieselbe Quelle haben; der Standardwert ist true.

**Returns:**
boolean
### getSaveHtmlAsZip() {#getSaveHtmlAsZip--}
```
public boolean getSaveHtmlAsZip()
```


Liefert, ob HTML‑Dateien als ZIP‑Archiv gespeichert werden sollen, der Standardwert ist false.

**Returns:**
boolean
### getShowChartSheet() {#getShowChartSheet--}
```
public boolean getShowChartSheet()
```


Ermittelt, ob das Diagramm‑Arbeitsblatt angezeigt wird. Der Standardwert ist false.

**Returns:**
boolean
### getSkipInvisibleShapes() {#getSkipInvisibleShapes--}
```
public boolean getSkipInvisibleShapes()
```


Liefert, ob Formen, die für die UI unsichtbar sind, übersprungen werden sollen, der Standardwert ist true.

**Returns:**
boolean
### getUsePrintArea() {#getUsePrintArea--}
```
public boolean getUsePrintArea()
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
public boolean isCollaborative()
```


Liefert, ob kollaboratives Bearbeiten unterstützt wird, der Standardwert ist false.

**Returns:**
boolean
### isWasm() {#isWasm--}
```
public boolean isWasm()
```


Ermittelt, ob GridJs in einem Browser‑WebAssembly‑Host anstelle eines Serverprozesses ausgeführt wird. Wenn true, wird kein FileCacheDirectory‑/Disk‑/Interrupt‑Thread‑Pfad verwendet, und der Dateicache muss von CacheImp stammen, da ein Browser‑Host keinen lokalen Datenträger hat. Der Codepfad wird zur Laufzeit ausgewählt, sodass eine Aspose.Cells.GridJs.dll beide Hosts bedient. Der Standardwert ist false.

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
public void setAutoFitColumnsOnLoad(boolean value)
```


Gibt an, ob die Spaltenbreite beim Laden der Datei automatisch angepasst werden soll, der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAutoFitRowsHeightOnLoad(boolean value) {#setAutoFitRowsHeightOnLoad-boolean-}
```
public void setAutoFitRowsHeightOnLoad(boolean value)
```


Gibt an, ob die Zeilenhöhe beim Laden der Datei automatisch angepasst werden soll, der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAutoOptimizeForLargeCells(boolean value) {#setAutoOptimizeForLargeCells-boolean-}
```
public void setAutoOptimizeForLargeCells(boolean value)
```


Legt fest, ob die Ladeleistung für Arbeitsblätter mit großen Zellen automatisch optimiert wird. Es werden einige Stile/Grenzen ignoriert, um die Ladezeit zu verkürzen. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setBaseRouteName(String value) {#setBaseRouteName-java.lang.String-}
```
public void setBaseRouteName(String value)
```


Legt den Basisnamen der Routen‑URL für den GridJs‑Controller fest. Der Standard ist GridJs2.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCollaborative(boolean value) {#setCollaborative-boolean-}
```
public void setCollaborative(boolean value)
```


Legt fest, ob kollaboratives Bearbeiten unterstützt wird, der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEmptySheetMaxCol(int value) {#setEmptySheetMaxCol-int-}
```
public void setEmptySheetMaxCol(int value)
```


Legt die maximale Standardspaltenzahl für ein leeres Arbeitsblatt fest. Der Standardwert ist 15.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setEmptySheetMaxRow(int value) {#setEmptySheetMaxRow-int-}
```
public void setEmptySheetMaxRow(int value)
```


Legt die maximale Standardzeilenzahl für ein leeres Arbeitsblatt fest. Der Standardwert ist 12.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setEnableChartClientRendering(boolean value) {#setEnableChartClientRendering-boolean-}
```
public void setEnableChartClientRendering(boolean value)
```


Legt fest, ob die clientseitige Diagrammdarstellung aktiviert wird. Wenn false, gibt GridJs nur Diagrammbilder/-formen aus und erfordert keine clientseitige Diagrammdarstellung. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFileCacheDirectory(String value) {#setFileCacheDirectory-java.lang.String-}
```
public void setFileCacheDirectory(String value)
```


Legt das Cache‑Verzeichnis zum Speichern von Tabellenkalkulationsdateien fest. Wir müssen es vor der Verwendung von GridJs auf einen bestimmten Pfad setzen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setFontFolders(String[] value) {#setFontFolders-java.lang.String---}
```
public void setFontFolders(String[] value)
```


Legt die Schriftordner für Schriften in gerenderten Bildern/Formen fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String[] |  |

### setIgnoreEmptyContent(boolean value) {#setIgnoreEmptyContent-boolean-}
```
public void setIgnoreEmptyContent(boolean value)
```


Legt fest, ob der maximale Bereich, der Daten, Stil, zusammengeführte Zellen und Formen enthält, angezeigt wird. Wenn die letzte Zeile oder Spalte Zellen ohne Wert und Formel, aber mit benutzerdefiniertem Stil enthält, wird diese Zeile/Spalte nicht angezeigt, wenn dieser Wert true ist\\u9286?\* Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setIslimitShapeOrImage(boolean value) {#setIslimitShapeOrImage-boolean-}
```
public void setIslimitShapeOrImage(boolean value)
```


Legt fest, ob die Gesamtzahl der angezeigten Formen/Bilder in einem Arbeitsblatt begrenzt werden soll; ist der Wert true, begrenzt GridJs die Gesamtzahl der angezeigten Formen oder Bilder in einem Arbeitsblatt auf MaxShapeOrImageCount. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setJsonCache(JsonCacheOptions value) {#setJsonCache-com.aspose.gridjs.JsonCacheOptions-}
```
public void setJsonCache(JsonCacheOptions value)
```


Legt die JSON‑Cache‑Konfigurationsoptionen fest. Steuert sowohl das Speicher‑ (L1) als auch das Festplatten‑ (L2) Cache‑Verhalten für das erzeugte Arbeitsbuch‑JSON.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions) |  |

### setLazyLoading(boolean value) {#setLazyLoading-boolean-}
```
public void setLazyLoading(boolean value)
```


Legt fest, ob nur das aktive Arbeitsblatt geladen werden soll, der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setMaxPdfSaveSeconds(int value) {#setMaxPdfSaveSeconds-int-}
```
public void setMaxPdfSaveSeconds(int value)
```


Legt die maximalen Zeitüberschreitungssekunden beim Speichern als PDF fest. Der Standardwert ist 10.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMaxShapeOrImageCount(int value) {#setMaxShapeOrImageCount-int-}
```
public void setMaxShapeOrImageCount(int value)
```


Legt die Gesamtanzahl der angezeigten Formen oder Bilder im aktiven Blatt fest, wirksam wenn IslimitShapeOrImage=true. Der Standardwert ist 100.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMaxShapeOrImageWidthOrHeight(int value) {#setMaxShapeOrImageWidthOrHeight-int-}
```
public void setMaxShapeOrImageWidthOrHeight(int value)
```


Legt die maximale Breite oder Höhe für eine Form oder ein Bild fest; GridJs ignoriert Formen oder Bilder, deren Breite oder Höhe größer ist, wirksam wenn IslimitShapeOrImage=true. Der Standardwert ist 10000.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMaxTotalShapeOrImageCount(int value) {#setMaxTotalShapeOrImageCount-int-}
```
public void setMaxTotalShapeOrImageCount(int value)
```


Legt die Gesamtanzahl der angezeigten Formen oder Bilder im Arbeitsbuch fest, wirksam wenn IslimitShapeOrImage=true. Der Standardwert ist 300.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMessageTopic(String value) {#setMessageTopic-java.lang.String-}
```
public void setMessageTopic(String value)
```


Legt die Websocket‑Ziele fest, die mit "\/topic" beginnen. Der Standard ist "\/topic/opr". Wird nur im kollaborativen Modus verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setPictureCacheDirectory(String value) {#setPictureCacheDirectory-java.lang.String-}
```
public void setPictureCacheDirectory(String value)
```


Legt das Cache‑Verzeichnis für Bilder fest (dies wirkt, wenn GridJsWorkbook.CacheImp null ist). Der Standardpfad ist "\\_piccache" im FileCacheDirectory.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setSameImageDetecting(boolean value) {#setSameImageDetecting-boolean-}
```
public void setSameImageDetecting(boolean value)
```


Legt fest, ob geprüft wird, ob Bilder dieselbe Quelle haben, der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSaveHtmlAsZip(boolean value) {#setSaveHtmlAsZip-boolean-}
```
public void setSaveHtmlAsZip(boolean value)
```


Legt fest, ob HTML-Dateien als ZIP-Archiv gespeichert werden, der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowChartSheet(boolean value) {#setShowChartSheet-boolean-}
```
public void setShowChartSheet(boolean value)
```


Legt fest, ob das Diagramm‑Arbeitsblatt angezeigt wird. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSkipInvisibleShapes(boolean value) {#setSkipInvisibleShapes-boolean-}
```
public void setSkipInvisibleShapes(boolean value)
```


Legt fest, ob Formen, die für die UI unsichtbar sind, übersprungen werden, der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setUsePrintArea(boolean value) {#setUsePrintArea-boolean-}
```
public void setUsePrintArea(boolean value)
```


Legt fest, ob PageSetup.PrintArea für den UI‑Anzeigebereich verwendet wird, wenn das Arbeitsblatt eine PageSetup‑Einstellung für PrintArea hat. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setWasm(boolean value) {#setWasm-boolean-}
```
public void setWasm(boolean value)
```


Legt fest, ob GridJs in einem Browser‑WebAssembly‑Host anstelle eines Serverprozesses ausgeführt wird. Wenn true, wird kein FileCacheDirectory‑/Disk‑/Interrupt‑Thread‑Pfad verwendet, und der Dateicache muss von CacheImp stammen, da ein Browser‑Host keinen lokalen Datenträger hat. Der Codepfad wird zur Laufzeit ausgewählt, sodass eine Aspose.Cells.GridJs.dll beide Hosts bedient. Der Standardwert ist false.

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

