---
title: "GridHtmlSaveOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Optionen zum Speichern einer HTML-Datei dar."
type: docs
url: /de/java/com.aspose.gridweb/gridhtmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions)
```
public class GridHtmlSaveOptions extends GridSaveOptions
```

Stellt die Optionen zum Speichern einer HTML-Datei dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [GridHtmlSaveOptions()](#GridHtmlSaveOptions--) | Erstellt Optionen zum Speichern einer HTML-Datei. |
| [GridHtmlSaveOptions(int format)](#GridHtmlSaveOptions-int-) | Erstellt Optionen zum Speichern einer HTM-Datei. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | Das Verzeichnis, in dem die angehängten Dateien gespeichert werden. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | Geben Sie das URL-Präfix für angehängte Dateien wie Bilder in der HTML-Datei an. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Der zwischengespeicherte Ordner wird verwendet, um große Daten zu speichern. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Leert die Arbeitsmappe nach dem Speichern der Datei. |
| [getCreateDirectory()](#getCreateDirectory--) | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt. |
| [getDefaultFontName()](#getDefaultFontName--) | Geben Sie den Standard-Schriftartnamen für den Export von HTML an; die Standardschriftart wird verwendet, wenn die Schriftart des Stils nicht vorhanden ist. Ist diese Eigenschaft null, verwendet Aspose.Cells eine universelle Schriftart, die dieselbe Familie wie die Originalschriftart hat. Der Standardwert ist null. |
| [getEncoding()](#getEncoding--) | Falls nicht festgelegt, wird Encoding.UTF8 als Standard‑Kodierungstyp verwendet. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | Gibt an, ob das gesamte Arbeitsbuch in eine HTML-Datei exportiert wird. |
| [getExportArea()](#getExportArea--) | Ruft den zu exportierenden CellArea des aktuell aktiven Arbeitsblatts ab. |
| [getExportGridLines()](#getExportGridLines--) | Gibt an, ob Rasterlinien exportiert werden. Der Standardwert ist false. |
| [getExportHeadings()](#getExportHeadings--) | Gibt an, ob Überschriften beim Speichern der Datei als HTML exportiert werden. Der Standardwert ist false. |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--) | Gibt an, ob der Inhalt ausgeblendeter Arbeitsblätter exportiert wird. Der Standardwert ist true. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | Legt fest, ob Bilder im Base64‑Format in HTML, MHTML oder EPUB gespeichert werden. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | Gibt an, ob nur der Druckbereich in eine HTML‑Datei exportiert wird. |
| [getExportSingleTab()](#getExportSingleTab--) | Gibt an, ob das einzelne Tabellenblatt exportiert wird, wenn die Datei nur ein Arbeitsblatt enthält. |
| [getMergeAreas()](#getMergeAreas--) | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden. |
| [getPageTitle()](#getPageTitle--) | Der Titel der HTML‑Seite. |
|  | [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | HTML-Tag in Zelle parsen, wie |

, als Zellenwert oder als HTML-Tag, Standard ist true |
| [getPresentationPreference()](#getPresentationPreference--) | Gibt an, ob HTML- oder MHT-Datei die bevorzugte Darstellung ist. Der Standardwert ist false. Wenn Sie eine schönere Darstellung wünschen, setzen Sie den Wert auf true. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Gibt an, ob Diagramm-Cache-Daten aktualisiert werden. |
| [getSaveFormat()](#getSaveFormat--) | Ermittelt das Speicherdateiformat. |
| [getSortNames()](#getSortNames--) | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden. |
| [hashCode()](#hashCode--) |  |
| [isExportComments()](#isExportComments--) | Gibt an, ob Kommentare beim Speichern der Datei nach HTML exportiert werden; der Standardwert ist false. |
| [isFullPathLink()](#isFullPathLink--) | Gibt an, ob ein vollständiger Pfadlink in sheet00x.htm, filelist.xml und tabstrip.htm verwendet wird. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | Das Verzeichnis, in dem die angehängten Dateien gespeichert werden. |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | Geben Sie das URL-Präfix für angehängte Dateien wie Bilder in der HTML-Datei an. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Der zwischengespeicherte Ordner wird verwendet, um große Daten zu speichern. |
| [setClearData(boolean value)](#setClearData-boolean-) | Leert die Arbeitsmappe nach dem Speichern der Datei. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Geben Sie den Standard-Schriftartnamen für den Export von HTML an; die Standardschriftart wird verwendet, wenn die Schriftart des Stils nicht vorhanden ist. Ist diese Eigenschaft null, verwendet Aspose.Cells eine universelle Schriftart, die dieselbe Familie wie die Originalschriftart hat. Der Standardwert ist null. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.gridweb.Encoding-) | Falls nicht festgelegt, wird Encoding.UTF8 als Standard‑Kodierungstyp verwendet. |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | Gibt an, ob das gesamte Arbeitsbuch in eine HTML-Datei exportiert wird. |
| [setExportArea(GridCellArea value)](#setExportArea-com.aspose.gridweb.GridCellArea-) | Legt den zu exportierenden CellArea des aktuell aktiven Arbeitsblatts fest. |
| [setExportComments(boolean value)](#setExportComments-boolean-) | Gibt an, ob Kommentare beim Speichern der Datei nach HTML exportiert werden; der Standardwert ist false. |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | Gibt an, ob Rasterlinien exportiert werden. Der Standardwert ist false. |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | Gibt an, ob Überschriften beim Speichern der Datei als HTML exportiert werden. Der Standardwert ist false. |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | Gibt an, ob der Inhalt ausgeblendeter Arbeitsblätter exportiert wird. Der Standardwert ist true. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | Legt fest, ob Bilder im Base64‑Format in HTML, MHTML oder EPUB gespeichert werden. |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | Gibt an, ob nur der Druckbereich in eine HTML‑Datei exportiert wird. |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | Gibt an, ob das einzelne Tabellenblatt exportiert wird, wenn die Datei nur ein Arbeitsblatt enthält. |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | Gibt an, ob ein vollständiger Pfadlink in sheet00x.htm, filelist.xml und tabstrip.htm verwendet wird. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden. |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | Der Titel der HTML‑Seite. |
|  | [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | HTML-Tag in Zelle parsen, wie |

, als Zellenwert oder als HTML-Tag, Standard ist true |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | Gibt an, ob HTML- oder MHT-Datei die bevorzugte Darstellung ist. Der Standardwert ist false. Wenn Sie eine schönere Darstellung wünschen, setzen Sie den Wert auf true. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Gibt an, ob Diagramm-Cache-Daten aktualisiert werden. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridHtmlSaveOptions() {#GridHtmlSaveOptions--}
```
public GridHtmlSaveOptions()
```


Erstellt Optionen zum Speichern einer HTML-Datei.

### GridHtmlSaveOptions(int format) {#GridHtmlSaveOptions-int-}
```
public GridHtmlSaveOptions(int format)
```


Erstellt Optionen zum Speichern einer HTM-Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). Das Speicherdateiformat. |

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
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


Das Verzeichnis, in dem die angehängten Dateien gespeichert werden. Nur beim Speichern in einen HTML‑Stream.

**Returns:**
java.lang.String
### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}
```
public String getAttachedFilesUrlPrefix()
```


Gibt das URL‑Präfix für angehängte Dateien wie Bilder in der HTML‑Datei an. Nur beim Speichern in einen HTML‑Stream.

**Returns:**
java.lang.String
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Der zwischengespeicherte Ordner wird verwendet, um große Daten zu speichern.

**Returns:**
java.lang.String
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
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Geben Sie den Standard-Schriftartnamen für den Export von HTML an; die Standardschriftart wird verwendet, wenn die Schriftart des Stils nicht vorhanden ist. Ist diese Eigenschaft null, verwendet Aspose.Cells eine universelle Schriftart, die dieselbe Familie wie die Originalschriftart hat. Der Standardwert ist null.

**Returns:**
java.lang.String
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Falls nicht festgelegt, wird Encoding.UTF8 als Standard‑Kodierungstyp verwendet.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding)
### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}
```
public boolean getExportActiveWorksheetOnly()
```


Gibt an, ob das gesamte Arbeitsbuch in eine HTML-Datei exportiert wird.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public GridCellArea getExportArea()
```


Ermittelt den zu exportierenden CellArea des aktuell aktiven Arbeitsblatts. Wenn Sie dieses Attribut setzen, wird der Druckbereich des aktuell aktiven Arbeitsblatts weggelassen. Nur der angegebene Bereich wird beim Speichern der Datei als HTML exportiert.

**Returns:**
[GridCellArea](../../com.aspose.gridweb/gridcellarea)
### getExportGridLines() {#getExportGridLines--}
```
public boolean getExportGridLines()
```


Gibt an, ob Rasterlinien exportiert werden. Der Standardwert ist false.

**Returns:**
boolean
### getExportHeadings() {#getExportHeadings--}
```
public boolean getExportHeadings()
```


Gibt an, ob Überschriften beim Speichern der Datei als HTML exportiert werden. Der Standardwert ist false. Wenn Sie die HTML-Datei nach Excel importieren möchten, behalten Sie den Standardwert bei.

**Returns:**
boolean
### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}
```
public boolean getExportHiddenWorksheet()
```


Gibt an, ob der Inhalt ausgeblendeter Arbeitsblätter exportiert wird. Der Standardwert ist true.

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


Legt fest, ob Bilder im Base64‑Format in HTML, MHTML oder EPUB gespeichert werden.

**Remarks**

Wenn diese Eigenschaft auf true gesetzt ist, werden Bilddaten direkt in den img‑Elementen exportiert und separate Dateien werden nicht erstellt.

**Returns:**
boolean
### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}
```
public boolean getExportPrintAreaOnly()
```


Gibt an, ob nur der Druckbereich in die HTML‑Datei exportiert wird. Der Standardwert ist false.

**Returns:**
boolean
### getExportSingleTab() {#getExportSingleTab--}
```
public boolean getExportSingleTab()
```


Gibt an, ob das einzelne Tabellenblatt exportiert wird, wenn die Datei nur ein Arbeitsblatt enthält. Der Standardwert ist false.

**Returns:**
boolean
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden.

**Remarks**

Der Standardwert ist false.

**Returns:**
boolean
### getPageTitle() {#getPageTitle--}
```
public String getPageTitle()
```


Der Titel der HTML-Seite. Nur beim Speichern in einen HTML-Stream.

**Returns:**
java.lang.String
### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}
```
public boolean getParseHtmlTagInCell()
```


HTML-Tag in Zelle parsen, wie

, als Zellenwert oder als HTML-Tag, Standard ist true

**Returns:**
boolean
### getPresentationPreference() {#getPresentationPreference--}
```
public boolean getPresentationPreference()
```


Gibt an, ob HTML- oder MHT-Datei die bevorzugte Darstellung ist. Der Standardwert ist false. Wenn Sie eine schönere Darstellung wünschen, setzen Sie den Wert auf true.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Gibt an, ob Diagramm-Cache-Daten aktualisiert werden.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Ermittelt das Speicherdateiformat.

Siehe [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat).

**Returns:**
int
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden.

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
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isExportComments() {#isExportComments--}
```
public boolean isExportComments()
```


Gibt an, ob Kommentare beim Speichern der Datei nach HTML exportiert werden; der Standardwert ist false.

**Returns:**
boolean
### isFullPathLink() {#isFullPathLink--}
```
public boolean isFullPathLink()
```


Gibt an, ob ein vollständiger Pfadlink in sheet00x.htm, filelist.xml und tabstrip.htm verwendet wird. Der Standardwert ist false.

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




### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


Das Verzeichnis, in dem die angehängten Dateien gespeichert werden. Nur beim Speichern in einen HTML‑Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```


Gibt das URL‑Präfix für angehängte Dateien wie Bilder in der HTML‑Datei an. Nur beim Speichern in einen HTML‑Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


Der zwischengespeicherte Ordner wird verwendet, um große Daten zu speichern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

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

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Geben Sie den Standard-Schriftartnamen für den Export von HTML an; die Standardschriftart wird verwendet, wenn die Schriftart des Stils nicht vorhanden ist. Ist diese Eigenschaft null, verwendet Aspose.Cells eine universelle Schriftart, die dieselbe Familie wie die Originalschriftart hat. Der Standardwert ist null.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.gridweb.Encoding-}
```
public void setEncoding(Encoding value)
```


Falls nicht festgelegt, wird Encoding.UTF8 als Standard‑Kodierungstyp verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.gridweb/encoding) |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


Gibt an, ob das gesamte Arbeitsbuch in eine HTML-Datei exportiert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportArea(GridCellArea value) {#setExportArea-com.aspose.gridweb.GridCellArea-}
```
public void setExportArea(GridCellArea value)
```


Legt den zu exportierenden CellArea des aktuell aktiven Arbeitsblatts fest. Wenn Sie dieses Attribut setzen, wird der Druckbereich des aktuell aktiven Arbeitsblatts weggelassen. Nur der angegebene Bereich wird beim Speichern der Datei als HTML exportiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GridCellArea](../../com.aspose.gridweb/gridcellarea) |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


Gibt an, ob Kommentare beim Speichern der Datei nach HTML exportiert werden; der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```


Gibt an, ob Rasterlinien exportiert werden. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```


Gibt an, ob Überschriften beim Speichern der Datei als HTML exportiert werden. Der Standardwert ist false. Wenn Sie die HTML-Datei nach Excel importieren möchten, behalten Sie den Standardwert bei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```


Gibt an, ob der Inhalt ausgeblendeter Arbeitsblätter exportiert wird. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


Legt fest, ob Bilder im Base64‑Format in HTML, MHTML oder EPUB gespeichert werden.

**Remarks**

Wenn diese Eigenschaft auf true gesetzt ist, werden Bilddaten direkt in den img‑Elementen exportiert und separate Dateien werden nicht erstellt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


Gibt an, ob nur der Druckbereich in die HTML‑Datei exportiert wird. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```


Gibt an, ob das einzelne Tabellenblatt exportiert wird, wenn die Datei nur ein Arbeitsblatt enthält. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


Gibt an, ob ein vollständiger Pfadlink in sheet00x.htm, filelist.xml und tabstrip.htm verwendet wird. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```


Der Titel der HTML-Seite. Nur beim Speichern in einen HTML-Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```


HTML-Tag in Zelle parsen, wie

, als Zellenwert oder als HTML-Tag, Standard ist true

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```


Gibt an, ob HTML- oder MHT-Datei die bevorzugte Darstellung ist. Der Standardwert ist false. Wenn Sie eine schönere Darstellung wünschen, setzen Sie den Wert auf true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Gibt an, ob Diagramm-Cache-Daten aktualisiert werden.

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

