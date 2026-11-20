---
title: "MarkdownSaveOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Speicheroptionen für Markdown dar."
type: docs
url: /de/java/com.aspose.cells/markdownsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class MarkdownSaveOptions extends SaveOptions
```

Stellt die Speicheroptionen für Markdown dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [MarkdownSaveOptions()](#MarkdownSaveOptions--) | Erstellt Optionen zum Speichern eines Markdown-Dokuments |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlignColumnPadding()](#getAlignColumnPadding--) | Gibt an, ob die Spaltenausrichtung für generierte Markdown-Tabellen aktiviert ist. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können. |
| [getCalculateFormula()](#getCalculateFormula--) | Gibt an, ob Formeln vor dem Speichern der Markdown-Datei berechnet werden sollen. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Leert die Arbeitsmappe nach dem Speichern der Datei. |
| [getCreateDirectory()](#getCreateDirectory--) | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt. |
| [getEncoding()](#getEncoding--) | Ruft die Standardkodierung ab. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. |
| [getExportHyperlinkAsReference()](#getExportHyperlinkAsReference--) | Gibt an, ob Hyperlinks mithilfe von Referenzdefinitionen statt im Inline-Format exportiert werden sollen. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | Gibt an, ob Bilder im Base64-Format in Markdown gespeichert werden. |
| [getFormatStrategy()](#getFormatStrategy--) | Liefert die Formatstrategie beim Exportieren des Zellwerts als Zeichenfolge. |
| [getImageOptions()](#getImageOptions--) | Rufen Sie das ImageOrPrintOptions‑Objekt vor dem Exportieren ab. |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | Der Datenanbieter, der Zellen­daten zum Speichern der Arbeitsmappe im Light‑Modus bereitstellt. |
| [getLineSeparator()](#getLineSeparator--) | Liefert den Zeilen­separator. |
| [getMergeAreas()](#getMergeAreas--) | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden. |
| [getOfficeMathOutputType()](#getOfficeMathOutputType--) | Gibt an, wie OfficeMath‑Objekte nach Markdown exportiert werden, Standardwert ist Bild. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen. |
| [getSaveFormat()](#getSaveFormat--) | Ermittelt das Speicherdateiformat. |
| [getSheetSet()](#getSheetSet--) | Ruft die zu rendernden Arbeitsblätter ab. |
| [getSortExternalNames()](#getSortExternalNames--) | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden. |
| [getSortNames()](#getSortNames--) | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden. |
| [getSplitTablesByBlankRow()](#getSplitTablesByBlankRow--) | Gibt an, ob leere Zeilen im Arbeitsblatt beim Export nach Markdown als Tabellentrenner behandelt werden sollen. |
| [getStreamProvider()](#getStreamProvider--) | Ruft den IStreamProvider zum Exportieren von Objekten ab. |
| [getTableHeaderType()](#getTableHeaderType--) | Liefert, wie die Kopfzeile der Tabelle festgelegt wird. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Gibt an, ob die SmartArt-Einstellungen aktualisiert werden. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden. |
| [getWarningCallback()](#getWarningCallback--) | Liest den Warn‑Callback. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignColumnPadding(char value)](#setAlignColumnPadding-char-) | Gibt an, ob die Spaltenausrichtung für generierte Markdown-Tabellen aktiviert ist. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Gibt an, ob Formeln vor dem Speichern der Markdown-Datei berechnet werden sollen. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [setClearData(boolean value)](#setClearData-boolean-) | Leert die Arbeitsmappe nach dem Speichern der Datei. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Legt die Standardkodierung fest. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. |
| [setExportHyperlinkAsReference(boolean value)](#setExportHyperlinkAsReference-boolean-) | Gibt an, ob Hyperlinks mithilfe von Referenzdefinitionen statt im Inline-Format exportiert werden sollen. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | Gibt an, ob Bilder im Base64-Format in Markdown gespeichert werden. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Legt die Formatstrategie beim Exportieren des Zellwerts als Zeichenfolge fest. |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | Der Datenanbieter, der Zellen­daten zum Speichern der Arbeitsmappe im Light‑Modus bereitstellt. |
| [setLineSeparator(String value)](#setLineSeparator-java.lang.String-) | Legt den Zeilen­separator fest. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden. |
| [setOfficeMathOutputType(int value)](#setOfficeMathOutputType-int-) | Gibt an, wie OfficeMath‑Objekte nach Markdown exportiert werden, Standardwert ist Bild. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Legt die zu rendernden Arbeitsblätter fest. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden. |
| [setSplitTablesByBlankRow(boolean value)](#setSplitTablesByBlankRow-boolean-) | Gibt an, ob leere Zeilen im Arbeitsblatt beim Export nach Markdown als Tabellentrenner behandelt werden sollen. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Legt den IStreamProvider für das Exportieren von Objekten fest. |
| [setTableHeaderType(int value)](#setTableHeaderType-int-) | Legt fest, wie die Kopfzeile der Tabelle gesetzt wird. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Gibt an, ob die SmartArt-Einstellungen aktualisiert werden. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Legt die Warn‑Callback‑Funktion fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### MarkdownSaveOptions() {#MarkdownSaveOptions--}
```
public MarkdownSaveOptions()
```


Erstellt Optionen zum Speichern eines Markdown-Dokuments

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
### getAlignColumnPadding() {#getAlignColumnPadding--}
```
public char getAlignColumnPadding()
```


Gibt an, ob die Spaltenausrichtung für erzeugte Markdown‑Tabellen aktiviert ist. Ist sie aktiviert, werden die Spalten durch Auffüllen des Zelleninhalts mit dem angegebenen Zeichen (typischerweise ' ' für Leerzeichen) ausgerichtet. Setzen Sie den Wert auf '\\0', um die Spaltenausrichtung zu deaktivieren (Standard).

**Returns:**
char
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können.

**Remarks**

Wenn der Ordner nicht angegeben wurde, ist der Standardwert dafür [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Wenn sein Standardwert null oder leer ist oder als null oder leer angegeben wurde, wird beim Speichern der Arbeitsmappe keine Cache‑Datei verwendet.

**Returns:**
java.lang.String
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


Gibt an, ob Formeln vor dem Speichern der Markdown-Datei berechnet werden sollen.

**Remarks**

Der Standardwert ist false.

**Returns:**
boolean
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
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Ruft die Standardkodierung ab.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. Der Standardwert ist true.

**Remarks**

Nur für .xls, .xlsx, .xlsb und .xlsm-Dateien.

**Returns:**
boolean
### getExportHyperlinkAsReference() {#getExportHyperlinkAsReference--}
```
public boolean getExportHyperlinkAsReference()
```


Gibt an, ob Hyperlinks mittels Referenzdefinitionen statt im Inline‑Format exportiert werden sollen. Der Standardwert ist false.

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


Gibt an, ob Bilder im Base64‑Format nach Markdown gespeichert werden. Der Standardwert ist true.

**Remarks**

Wenn diese Eigenschaft auf true gesetzt ist, werden Bilddaten direkt in den img‑Elementen exportiert und separate Dateien werden nicht erstellt.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Liefert die Formatstrategie beim Exportieren des Zellwerts als Zeichenfolge.

Siehe [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Returns:**
int
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


Rufen Sie das ImageOrPrintOptions‑Objekt vor dem Exportieren ab.

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
### getLightCellsDataProvider() {#getLightCellsDataProvider--}
```
public LightCellsDataProvider getLightCellsDataProvider()
```


Der Datenanbieter, der Zellen­daten zum Speichern der Arbeitsmappe im Light‑Modus bereitstellt.

**Returns:**
[LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider)
### getLineSeparator() {#getLineSeparator--}
```
public String getLineSeparator()
```


Liefert den Zeilen­separator.

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
### getOfficeMathOutputType() {#getOfficeMathOutputType--}
```
public int getOfficeMathOutputType()
```


Gibt an, wie OfficeMath‑Objekte nach Markdown exportiert werden, Standardwert ist Bild.

Siehe [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

**Returns:**
int
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
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Liefert die zu rendernden Tabellen. Standard ist alle sichtbaren Tabellen in der Arbeitsmappe: [SheetSet.getActive()](../../com.aspose.cells/sheetset\#getActive--).

**Remarks**

Das Set wird ignoriert, wenn es in [SheetRender](../../com.aspose.cells/sheetrender) verwendet wird

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
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
### getSplitTablesByBlankRow() {#getSplitTablesByBlankRow--}
```
public boolean getSplitTablesByBlankRow()
```


Gibt an, ob leere Zeilen im Arbeitsblatt beim Export nach Markdown als Tabellentrenner behandelt werden sollen. Der Standardwert ist false.

**Returns:**
boolean
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Liefert den IStreamProvider zum Exportieren von Objekten. Wenn `null`, werden die exportierten Objekte im selben Verzeichnis wie die Ausgabedatei gespeichert.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getTableHeaderType() {#getTableHeaderType--}
```
public int getTableHeaderType()
```


Liefert, wie die Kopfzeile der Tabelle festgelegt wird.

Siehe [MarkdownTableHeaderType](../../com.aspose.cells/markdowntableheadertype).

**Returns:**
int
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




### setAlignColumnPadding(char value) {#setAlignColumnPadding-char-}
```
public void setAlignColumnPadding(char value)
```


Gibt an, ob die Spaltenausrichtung für erzeugte Markdown‑Tabellen aktiviert ist. Ist sie aktiviert, werden die Spalten durch Auffüllen des Zelleninhalts mit dem angegebenen Zeichen (typischerweise ' ' für Leerzeichen) ausgerichtet. Setzen Sie den Wert auf '\\0', um die Spaltenausrichtung zu deaktivieren (Standard).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | char |  |

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

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Gibt an, ob Formeln vor dem Speichern der Markdown-Datei berechnet werden sollen.

**Remarks**

Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Legt die Standardkodierung fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

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

### setExportHyperlinkAsReference(boolean value) {#setExportHyperlinkAsReference-boolean-}
```
public void setExportHyperlinkAsReference(boolean value)
```


Gibt an, ob Hyperlinks mittels Referenzdefinitionen statt im Inline‑Format exportiert werden sollen. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


Gibt an, ob Bilder im Base64‑Format nach Markdown gespeichert werden. Der Standardwert ist true.

**Remarks**

Wenn diese Eigenschaft auf true gesetzt ist, werden Bilddaten direkt in den img‑Elementen exportiert und separate Dateien werden nicht erstellt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Legt die Formatstrategie beim Exportieren des Zellwerts als Zeichenfolge fest.

Siehe [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setLightCellsDataProvider(LightCellsDataProvider value) {#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-}
```
public void setLightCellsDataProvider(LightCellsDataProvider value)
```


Der Datenanbieter, der Zellen­daten zum Speichern der Arbeitsmappe im Light‑Modus bereitstellt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider) |  |

### setLineSeparator(String value) {#setLineSeparator-java.lang.String-}
```
public void setLineSeparator(String value)
```


Legt den Zeilen­separator fest.

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

### setOfficeMathOutputType(int value) {#setOfficeMathOutputType-int-}
```
public void setOfficeMathOutputType(int value)
```


Gibt an, wie OfficeMath‑Objekte nach Markdown exportiert werden, Standardwert ist Bild.

Siehe [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Legt die zu rendernden Tabellen fest. Standard ist alle sichtbaren Tabellen in der Arbeitsmappe: [SheetSet.getActive()](../../com.aspose.cells/sheetset\#getActive--).

**Remarks**

Das Set wird ignoriert, wenn es in [SheetRender](../../com.aspose.cells/sheetrender) verwendet wird

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

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

### setSplitTablesByBlankRow(boolean value) {#setSplitTablesByBlankRow-boolean-}
```
public void setSplitTablesByBlankRow(boolean value)
```


Gibt an, ob leere Zeilen im Arbeitsblatt beim Export nach Markdown als Tabellentrenner behandelt werden sollen. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Legt den IStreamProvider zum Exportieren von Objekten fest. Wenn `null`, werden die exportierten Objekte im selben Verzeichnis wie die Ausgabedatei gespeichert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setTableHeaderType(int value) {#setTableHeaderType-int-}
```
public void setTableHeaderType(int value)
```


Legt fest, wie die Kopfzeile der Tabelle gesetzt wird.

Siehe [MarkdownTableHeaderType](../../com.aspose.cells/markdowntableheadertype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

