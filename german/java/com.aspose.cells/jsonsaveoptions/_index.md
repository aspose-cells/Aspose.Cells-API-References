---
title: "JsonSaveOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Optionen zum Speichern der Arbeitsmappe als JSON-Datei dar."
type: docs
url: /de/java/com.aspose.cells/jsonsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class JsonSaveOptions extends SaveOptions
```

Stellt die Optionen zum Speichern der Arbeitsmappe als JSON-Datei dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [JsonSaveOptions()](#JsonSaveOptions--) | Erstellt Optionen zum Speichern einer JSON-Datei. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlwaysExportAsJsonObject()](#getAlwaysExportAsJsonObject--) | Gibt an, ob Excel immer als Objekt nach JSON exportiert wird, selbst wenn nur ein Arbeitsblatt in der Datei vorhanden ist. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Leert die Arbeitsmappe nach dem Speichern der Datei. |
| [getCreateDirectory()](#getCreateDirectory--) | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. |
| [getExportArea()](#getExportArea--) | Ermittelt den Exportbereich. |
| [getExportAsString()](#getExportAsString--) | Exportiert den Zeichenkettenwert der Zellen nach JSON. |
| [getExportEmptyCells()](#getExportEmptyCells--) | Gibt an, ob leere Zellen als null exportiert werden. |
| [getExportHyperlinkType()](#getExportHyperlinkType--) | Stellt den Typ des Hyperlink-Exports nach JSON dar. |
| [getExportNestedStructure()](#getExportNestedStructure--) | Exportiert als übergeordnete/untergeordnete hierarchische JSON-Struktur. |
| [getExportStylePool()](#getExportStylePool--) | Gibt an, ob Stile gesammelt oder einzeln für jede Zelle exportiert werden sollen. |
| [getIndent()](#getIndent--) | Gibt die Einrückung an. |
| [getMergeAreas()](#getMergeAreas--) | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen. |
| [getSaveFormat()](#getSaveFormat--) | Ermittelt das Speicherdateiformat. |
| [getSchemas()](#getSchemas--) | Das ursprüngliche JSON-Schema jedes Arbeitsblatts. |
| [getSheetIndexes()](#getSheetIndexes--) | Stellt die Indizes der exportierten Arbeitsblätter dar. |
| [getSkipEmptyRows()](#getSkipEmptyRows--) | Gibt an, ob leere Zeilen übersprungen werden. |
| [getSortExternalNames()](#getSortExternalNames--) | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden. |
| [getSortNames()](#getSortNames--) | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden. |
| [getToExcelStruct()](#getToExcelStruct--) | Gibt an, ob in die JSON-Struktur der Excel-Datei konvertiert wird. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Gibt an, ob die SmartArt-Einstellungen aktualisiert werden. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden. |
| [getWarningCallback()](#getWarningCallback--) | Liest den Warn‑Callback. |
| [hasHeaderRow()](#hasHeaderRow--) | Gibt an, ob der Bereich eine Kopfzeile enthält. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlwaysExportAsJsonObject(boolean value)](#setAlwaysExportAsJsonObject-boolean-) | Gibt an, ob Excel immer als Objekt nach JSON exportiert wird, selbst wenn nur ein Arbeitsblatt in der Datei vorhanden ist. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [setClearData(boolean value)](#setClearData-boolean-) | Leert die Arbeitsmappe nach dem Speichern der Datei. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Legt den Exportbereich fest. |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | Exportiert den Zeichenkettenwert der Zellen nach JSON. |
| [setExportEmptyCells(boolean value)](#setExportEmptyCells-boolean-) | Gibt an, ob leere Zellen als null exportiert werden. |
| [setExportHyperlinkType(int value)](#setExportHyperlinkType-int-) | Stellt den Typ des Hyperlink-Exports nach JSON dar. |
| [setExportNestedStructure(boolean value)](#setExportNestedStructure-boolean-) | Exportiert als übergeordnete/untergeordnete hierarchische JSON-Struktur. |
| [setExportStylePool(boolean value)](#setExportStylePool-boolean-) | Gibt an, ob Stile gesammelt oder einzeln für jede Zelle exportiert werden sollen. |
| [setHasHeaderRow(boolean value)](#setHasHeaderRow-boolean-) | Gibt an, ob der Bereich eine Kopfzeile enthält. |
| [setIndent(String value)](#setIndent-java.lang.String-) | Gibt die Einrückung an. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen. |
| [setSchemas(String[] value)](#setSchemas-java.lang.String---) | Das ursprüngliche JSON-Schema jedes Arbeitsblatts. |
| [setSheetIndexes(int[] value)](#setSheetIndexes-int---) | Stellt die Indizes der exportierten Arbeitsblätter dar. |
| [setSkipEmptyRows(boolean value)](#setSkipEmptyRows-boolean-) | Gibt an, ob leere Zeilen übersprungen werden. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden. |
| [setToExcelStruct(boolean value)](#setToExcelStruct-boolean-) | Gibt an, ob in die JSON-Struktur der Excel-Datei konvertiert wird. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Gibt an, ob die SmartArt-Einstellungen aktualisiert werden. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Legt die Warn‑Callback‑Funktion fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### JsonSaveOptions() {#JsonSaveOptions--}
```
public JsonSaveOptions()
```


Erstellt Optionen zum Speichern einer JSON-Datei.

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
### getAlwaysExportAsJsonObject() {#getAlwaysExportAsJsonObject--}
```
public boolean getAlwaysExportAsJsonObject()
```


Gibt an, ob Excel immer als Objekt nach JSON exportiert wird, selbst wenn nur ein Arbeitsblatt in der Datei vorhanden ist.

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
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt.

**Remarks**

Der Standardwert ist false.

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
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


Ermittelt den Exportbereich.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```


Exportiert den Zeichenkettenwert der Zellen nach JSON.

**Returns:**
boolean
### getExportEmptyCells() {#getExportEmptyCells--}
```
public boolean getExportEmptyCells()
```


Gibt an, ob leere Zellen als null exportiert werden.

**Returns:**
boolean
### getExportHyperlinkType() {#getExportHyperlinkType--}
```
public int getExportHyperlinkType()
```


Stellt den Typ des Hyperlink-Exports nach JSON dar.

Siehe [JsonExportHyperlinkType](../../com.aspose.cells/jsonexporthyperlinktype).

**Remarks**

Der Standardwert ist [JsonExportHyperlinkType.DISPLAY\_STRING](../../com.aspose.cells/jsonexporthyperlinktype\#DISPLAY-STRING);

**Returns:**
int
### getExportNestedStructure() {#getExportNestedStructure--}
```
public boolean getExportNestedStructure()
```


Exportiert als übergeordnete/untergeordnete hierarchische JSON-Struktur.

**Remarks**

**Returns:**
boolean
### getExportStylePool() {#getExportStylePool--}
```
public boolean getExportStylePool()
```


Gibt an, ob Stile gesammelt oder einzeln für jede Zelle exportiert werden sollen.

**Returns:**
boolean
### getIndent() {#getIndent--}
```
public String getIndent()
```


Gibt die Einrückung an.

**Remarks**

Wenn die Einrückung null oder leer ist, wird das exportierte json nicht formatiert.

**Returns:**
java.lang.String
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
### getSchemas() {#getSchemas--}
```
public String[] getSchemas()
```


Das ursprüngliche JSON-Schema jedes Arbeitsblatts.

**Returns:**
java.lang.String[]
### getSheetIndexes() {#getSheetIndexes--}
```
public int[] getSheetIndexes()
```


Stellt die Indizes der exportierten Arbeitsblätter dar.

**Returns:**
int[]
### getSkipEmptyRows() {#getSkipEmptyRows--}
```
public boolean getSkipEmptyRows()
```


Gibt an, ob leere Zeilen übersprungen werden.

**Returns:**
boolean
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
### getToExcelStruct() {#getToExcelStruct--}
```
public boolean getToExcelStruct()
```


Gibt an, ob in die JSON-Struktur der Excel-Datei konvertiert wird.

**Remarks**

Nur zum Konvertieren eines Bereichs nach JSON.

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
### hasHeaderRow() {#hasHeaderRow--}
```
public boolean hasHeaderRow()
```


Gibt an, ob der Bereich eine Kopfzeile enthält.

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




### setAlwaysExportAsJsonObject(boolean value) {#setAlwaysExportAsJsonObject-boolean-}
```
public void setAlwaysExportAsJsonObject(boolean value)
```


Gibt an, ob Excel immer als Objekt nach JSON exportiert wird, selbst wenn nur ein Arbeitsblatt in der Datei vorhanden ist.

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

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


Legt den Exportbereich fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


Exportiert den Zeichenkettenwert der Zellen nach JSON.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportEmptyCells(boolean value) {#setExportEmptyCells-boolean-}
```
public void setExportEmptyCells(boolean value)
```


Gibt an, ob leere Zellen als null exportiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportHyperlinkType(int value) {#setExportHyperlinkType-int-}
```
public void setExportHyperlinkType(int value)
```


Stellt den Typ des Hyperlink-Exports nach JSON dar.

Siehe [JsonExportHyperlinkType](../../com.aspose.cells/jsonexporthyperlinktype).

**Remarks**

Der Standardwert ist [JsonExportHyperlinkType.DISPLAY\_STRING](../../com.aspose.cells/jsonexporthyperlinktype\#DISPLAY-STRING);

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setExportNestedStructure(boolean value) {#setExportNestedStructure-boolean-}
```
public void setExportNestedStructure(boolean value)
```


Exportiert als übergeordnete/untergeordnete hierarchische JSON-Struktur.

**Remarks**

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportStylePool(boolean value) {#setExportStylePool-boolean-}
```
public void setExportStylePool(boolean value)
```


Gibt an, ob Stile gesammelt oder einzeln für jede Zelle exportiert werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHasHeaderRow(boolean value) {#setHasHeaderRow-boolean-}
```
public void setHasHeaderRow(boolean value)
```


Gibt an, ob der Bereich eine Kopfzeile enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setIndent(String value) {#setIndent-java.lang.String-}
```
public void setIndent(String value)
```


Gibt die Einrückung an.

**Remarks**

Wenn die Einrückung null oder leer ist, wird das exportierte json nicht formatiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

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

### setSchemas(String[] value) {#setSchemas-java.lang.String---}
```
public void setSchemas(String[] value)
```


Das ursprüngliche JSON-Schema jedes Arbeitsblatts.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String[] |  |

### setSheetIndexes(int[] value) {#setSheetIndexes-int---}
```
public void setSheetIndexes(int[] value)
```


Stellt die Indizes der exportierten Arbeitsblätter dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int[] |  |

### setSkipEmptyRows(boolean value) {#setSkipEmptyRows-boolean-}
```
public void setSkipEmptyRows(boolean value)
```


Gibt an, ob leere Zeilen übersprungen werden.

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

### setToExcelStruct(boolean value) {#setToExcelStruct-boolean-}
```
public void setToExcelStruct(boolean value)
```


Gibt an, ob in die JSON-Struktur der Excel-Datei konvertiert wird.

**Remarks**

Nur zum Konvertieren eines Bereichs nach JSON.

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

