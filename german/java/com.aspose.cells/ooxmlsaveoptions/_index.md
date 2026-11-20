---
title: "OoxmlSaveOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Optionen zum Speichern einer Office‑Open‑XML‑Datei dar."
type: docs
url: /de/java/com.aspose.cells/ooxmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class OoxmlSaveOptions extends SaveOptions
```

Stellt die Optionen zum Speichern einer Office‑Open‑XML‑Datei dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [OoxmlSaveOptions()](#OoxmlSaveOptions--) | Erstellt die Optionen zum Speichern von Office Open XML-Dateien. |
| [OoxmlSaveOptions(int saveFormat)](#OoxmlSaveOptions-int-) | Erstellt die Optionen zum Speichern von Office Open XML-Dateien. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAsFlatOpc()](#getAsFlatOpc--) | Gibt an, ob als flache OPC-Datei gespeichert wird, die vom Open XML SDK erzeugt werden kann. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Leert die Arbeitsmappe nach dem Speichern der Datei. |
| [getCompressionType()](#getCompressionType--) | Ermittelt den Kompressionstyp für ooxml-Datei. |
| [getCreateDirectory()](#getCreateDirectory--) | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt. |
| [getEmbedOoxmlAsOleObject()](#getEmbedOoxmlAsOleObject--) | Gibt an, ob Ooxml-Dateien von OleObject als Ole-Objekt eingebettet werden. |
| [getEnableZip64()](#getEnableZip64--) | Verwenden Sie ZIP64-Erweiterungen beim Schreiben von ZIP-Archiven, falls erforderlich. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. |
| [getExportCellName()](#getExportCellName--) | Gibt an, ob Zellnamen in Excel2007 .xlsx (.xlsm, .xltx, .xltm)-Dateien exportiert werden. |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | Der Datenanbieter zum Speichern der Arbeitsmappe im Light‑Modus. |
| [getMergeAreas()](#getMergeAreas--) | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen. |
| [getSaveFormat()](#getSaveFormat--) | Ermittelt das Speicherdateiformat. |
| [getSortExternalNames()](#getSortExternalNames--) | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden. |
| [getSortNames()](#getSortNames--) | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Gibt an, ob die SmartArt-Einstellungen aktualisiert werden. |
| [getUpdateZoom()](#getUpdateZoom--) | Gibt an, ob der Skalierungsfaktor vor dem Speichern der Datei aktualisiert wird, wenn die Eigenschaften PageSetup.FitToPagesWide und PageSetup.FitToPagesTall steuern, wie das Arbeitsblatt skaliert wird. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden. |
| [getWarningCallback()](#getWarningCallback--) | Liest den Warn‑Callback. |
| [getWpsCompatibility()](#getWpsCompatibility--) | Gibt an, ob die xls‑Datei stärker mit WPS kompatibel gemacht werden soll. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAsFlatOpc(boolean value)](#setAsFlatOpc-boolean-) | Gibt an, ob als flache OPC-Datei gespeichert wird, die vom Open XML SDK erzeugt werden kann. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [setClearData(boolean value)](#setClearData-boolean-) | Leert die Arbeitsmappe nach dem Speichern der Datei. |
| [setCompressionType(int value)](#setCompressionType-int-) | Legt den Kompressionstyp für ooxml-Datei fest. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt. |
| [setEmbedOoxmlAsOleObject(boolean value)](#setEmbedOoxmlAsOleObject-boolean-) | Gibt an, ob Ooxml-Dateien von OleObject als Ole-Objekt eingebettet werden. |
| [setEnableZip64(boolean value)](#setEnableZip64-boolean-) | Verwenden Sie ZIP64-Erweiterungen beim Schreiben von ZIP-Archiven, falls erforderlich. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. |
| [setExportCellName(boolean value)](#setExportCellName-boolean-) | Gibt an, ob Zellnamen in Excel2007 .xlsx (.xlsm, .xltx, .xltm)-Dateien exportiert werden. |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | Der Datenanbieter zum Speichern der Arbeitsmappe im Light‑Modus. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Gibt an, ob die SmartArt-Einstellungen aktualisiert werden. |
| [setUpdateZoom(boolean value)](#setUpdateZoom-boolean-) | Gibt an, ob der Skalierungsfaktor vor dem Speichern der Datei aktualisiert wird, wenn die Eigenschaften PageSetup.FitToPagesWide und PageSetup.FitToPagesTall steuern, wie das Arbeitsblatt skaliert wird. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Legt die Warn‑Callback‑Funktion fest. |
| [setWpsCompatibility(boolean value)](#setWpsCompatibility-boolean-) | Gibt an, ob die xls‑Datei stärker mit WPS kompatibel gemacht werden soll. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### OoxmlSaveOptions() {#OoxmlSaveOptions--}
```
public OoxmlSaveOptions()
```


Erstellt die Optionen zum Speichern von Office Open XML-Dateien.

### OoxmlSaveOptions(int saveFormat) {#OoxmlSaveOptions-int-}
```
public OoxmlSaveOptions(int saveFormat)
```


Erstellt die Optionen zum Speichern von Office Open XML-Dateien.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Das Dateiformat. Es sollte einer der folgenden Typen sein: [SaveFormat.XLSX](../../com.aspose.cells/saveformat\#XLSX), [SaveFormat.XLTX](../../com.aspose.cells/saveformat\#XLTX), [SaveFormat.XLAM](../../com.aspose.cells/saveformat\#XLAM), [SaveFormat.XLSM](../../com.aspose.cells/saveformat\#XLSM) oder [SaveFormat.XLTM](../../com.aspose.cells/saveformat\#XLTM), andernfalls wird das gespeicherte Format automatisch auf [SaveFormat.XLSX](../../com.aspose.cells/saveformat\#XLSX) gesetzt. |

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
### getAsFlatOpc() {#getAsFlatOpc--}
```
public boolean getAsFlatOpc()
```


Gibt an, ob als flache OPC-Datei gespeichert wird, die vom Open XML SDK erzeugt werden kann.

**Returns:**
boolean
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können.

**Remarks**

Wenn der Ordner nicht angegeben wurde, ist der Standardwert dafür [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Wenn sein Standardwert null oder leer ist oder als null oder leer angegeben wurde, wird beim Speichern der Arbeitsmappe keine Cache‑Datei verwendet.

**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Ob die Beschränkungen einer Excel-Datei geprüft werden, wenn der Benutzer Zellen-bezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht das Eingeben eines Zeichenfolgenwerts, der länger als 32 K ist. Wenn Sie einen Wert eingeben, der länger als 32 K ist, wird er abgeschnitten.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


Leert die Arbeitsmappe nach dem Speichern der Datei.

**Returns:**
boolean
### getCompressionType() {#getCompressionType--}
```
public int getCompressionType()
```


Ermittelt den Kompressionstyp für ooxml-Datei.

Siehe [OoxmlCompressionType](../../com.aspose.cells/ooxmlcompressiontype).

**Remarks**

Der Standardwert ist OoxmlCompressionType.Level2.

**Returns:**
int
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt.

**Remarks**

Der Standardwert ist false.

**Returns:**
boolean
### getEmbedOoxmlAsOleObject() {#getEmbedOoxmlAsOleObject--}
```
public boolean getEmbedOoxmlAsOleObject()
```


Gibt an, ob Ooxml-Dateien von OleObject als Ole-Objekt eingebettet werden.

**Remarks**

Nur für OleObject.

**Returns:**
boolean
### getEnableZip64() {#getEnableZip64--}
```
public boolean getEnableZip64()
```


Verwenden Sie ZIP64-Erweiterungen beim Schreiben von ZIP-Archiven, falls erforderlich.

**Returns:**
boolean
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. Der Standardwert ist true.

**Remarks**

Nur für .xls, .xlsx, .xlsb und .xlsm-Dateien.

**Returns:**
boolean
### getExportCellName() {#getExportCellName--}
```
public boolean getExportCellName()
```


Gibt an, ob Zellnamen in Excel2007 .xlsx (.xlsm, .xltx, .xltm)-Dateien exportiert werden. Wenn die Ausgabedatei von SQL Server DTS verwendet werden kann, muss dieser Wert true sein. Das Setzen des Wertes auf false erhöht die Leistung erheblich und reduziert die Dateigröße beim Erstellen großer Dateien. Der Standardwert ist true.

**Returns:**
boolean
### getLightCellsDataProvider() {#getLightCellsDataProvider--}
```
public LightCellsDataProvider getLightCellsDataProvider()
```


Der Datenanbieter zum Speichern der Arbeitsmappe im Light‑Modus.

**Returns:**
[LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider)
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden.

**Remarks**

Der Standardwert ist false.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Ermittelt das Speicherdateiformat.

Siehe [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden.

**Returns:**
boolean
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Gibt an, ob die Smart‑Art‑Einstellung aktualisiert wird. Der Standardwert ist false.

**Remarks**

Wirkt nur nach dem Aufruf der Methode Shape.GetResultOfSmartArt() und wenn die zwischengespeicherten Shapes in der Vorlagendatei vorhanden sind.

**Returns:**
boolean
### getUpdateZoom() {#getUpdateZoom--}
```
public boolean getUpdateZoom()
```


Gibt an, ob der Skalierungsfaktor vor dem Speichern der Datei aktualisiert wird, wenn die Eigenschaften PageSetup.FitToPagesWide und PageSetup.FitToPagesTall steuern, wie das Arbeitsblatt skaliert wird.

**Remarks**

Der Standardwert ist aus Leistungsgründen false.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden.

**Remarks**

Der Standardwert ist false.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Liest den Warn‑Callback.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWpsCompatibility() {#getWpsCompatibility--}
```
public boolean getWpsCompatibility()
```


Gibt an, ob die xls‑Datei stärker mit WPS kompatibel gemacht werden soll.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft WorkbookSetting.WpsCompatibility. Diese Methode wird 12 Monate später, seit Dezember 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAsFlatOpc(boolean value) {#setAsFlatOpc-boolean-}
```
public void setAsFlatOpc(boolean value)
```


Gibt an, ob als flache OPC-Datei gespeichert wird, die vom Open XML SDK erzeugt werden kann.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können.

**Remarks**

Wenn der Ordner nicht angegeben wurde, ist der Standardwert dafür [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Wenn sein Standardwert null oder leer ist oder als null oder leer angegeben wurde, wird beim Speichern der Arbeitsmappe keine Cache‑Datei verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Ob die Beschränkungen einer Excel-Datei geprüft werden, wenn der Benutzer Zellen-bezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht das Eingeben eines Zeichenfolgenwerts, der länger als 32 K ist. Wenn Sie einen Wert eingeben, der länger als 32 K ist, wird er abgeschnitten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Leert die Arbeitsmappe nach dem Speichern der Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCompressionType(int value) {#setCompressionType-int-}
```
public void setCompressionType(int value)
```


Legt den Kompressionstyp für ooxml-Datei fest.

Siehe [OoxmlCompressionType](../../com.aspose.cells/ooxmlcompressiontype).

**Remarks**

Der Standardwert ist OoxmlCompressionType.Level2.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt.

**Remarks**

Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEmbedOoxmlAsOleObject(boolean value) {#setEmbedOoxmlAsOleObject-boolean-}
```
public void setEmbedOoxmlAsOleObject(boolean value)
```


Gibt an, ob Ooxml-Dateien von OleObject als Ole-Objekt eingebettet werden.

**Remarks**

Nur für OleObject.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableZip64(boolean value) {#setEnableZip64-boolean-}
```
public void setEnableZip64(boolean value)
```


Verwenden Sie ZIP64-Erweiterungen beim Schreiben von ZIP-Archiven, falls erforderlich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. Der Standardwert ist true.

**Remarks**

Nur für .xls, .xlsx, .xlsb und .xlsm-Dateien.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportCellName(boolean value) {#setExportCellName-boolean-}
```
public void setExportCellName(boolean value)
```


Gibt an, ob Zellnamen in Excel2007 .xlsx (.xlsm, .xltx, .xltm)-Dateien exportiert werden. Wenn die Ausgabedatei von SQL Server DTS verwendet werden kann, muss dieser Wert true sein. Das Setzen des Wertes auf false erhöht die Leistung erheblich und reduziert die Dateigröße beim Erstellen großer Dateien. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setLightCellsDataProvider(LightCellsDataProvider value) {#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-}
```
public void setLightCellsDataProvider(LightCellsDataProvider value)
```


Der Datenanbieter zum Speichern der Arbeitsmappe im Light‑Modus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider) |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden.

**Remarks**

Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


Gibt an, ob die Smart‑Art‑Einstellung aktualisiert wird. Der Standardwert ist false.

**Remarks**

Wirkt nur nach dem Aufruf der Methode Shape.GetResultOfSmartArt() und wenn die zwischengespeicherten Shapes in der Vorlagendatei vorhanden sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setUpdateZoom(boolean value) {#setUpdateZoom-boolean-}
```
public void setUpdateZoom(boolean value)
```


Gibt an, ob der Skalierungsfaktor vor dem Speichern der Datei aktualisiert wird, wenn die Eigenschaften PageSetup.FitToPagesWide und PageSetup.FitToPagesTall steuern, wie das Arbeitsblatt skaliert wird.

**Remarks**

Der Standardwert ist aus Leistungsgründen false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden.

**Remarks**

Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Legt die Warn‑Callback‑Funktion fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### setWpsCompatibility(boolean value) {#setWpsCompatibility-boolean-}
```
public void setWpsCompatibility(boolean value)
```


Gibt an, ob die xls‑Datei stärker mit WPS kompatibel gemacht werden soll.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft WorkbookSetting.WpsCompatibility. Diese Methode wird 12 Monate später, seit Dezember 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

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

